# Data-views

var buffer = new ArrayBuffer(2);
var view = new DataView(buffer);
view.setUint8(0, 0xFF);
view.setUint8(1, 0x01);
console.log(view.getUint16(0, false)); // 65281
console.log(view.getUint16(0, true)); // 511
