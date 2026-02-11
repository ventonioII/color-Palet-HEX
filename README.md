# color-Palet-HEX

void _changeColor() {
tempColor = backgroundColor;

showDialog(
context: context,
builder: (context) => AlertDialog(
title: const Text('Chose color'),
content: SingleChildScrollView(
child: Column(
children: [
ColorPicker(
pickerColor: tempColor,
onColorChanged: (color) {
setState(() {
tempColor = color;
});
},
enableAlpha: false,
showLabel: true,
pickerAreaHeightPercent: 0.8,
),
