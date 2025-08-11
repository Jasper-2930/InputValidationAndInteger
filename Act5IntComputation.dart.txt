import 'dart:io';

void main() {
  stdout.write("Enter first number: ");
  var a = int.tryParse(stdin.readLineSync() ?? "");
  if (a == null) return print("Invalid input!");

  stdout.write("Enter second number: ");
  var b = int.tryParse(stdin.readLineSync() ?? "");
  if (b == null) return print("Invalid input!");

  print("Add: ${a + b}");
  print("Subtract: ${a - b}");
  print("Multiply: ${a * b}");
  if (b != 0) {
    print("Divide: ${a / b}");
  } else {
    print("Cannot divide by zero");
  }
}