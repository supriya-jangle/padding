import 'package:flutter/material.dart';
void main() => runApp(MyApp());
class MyApp extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
 return MaterialApp(
 home: PaddingContainerDemo(),
 );
 }
}
class PaddingContainerDemo extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
 return Scaffold(
 appBar: AppBar(title: Text('Container with Padding')),
 body: Center(
 child: Container(
 padding: EdgeInsets.all(20), // ⬅️ Adds space inside the 
container
 color: Colors.purpleAccent,
 child: Text(
 'With Padding',
 style: TextStyle(fontSize: 18, color: Colors.white),
 ),
 ),
 ),
 );
 }
