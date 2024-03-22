import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text('Mixed Widget Column Example'),
        ),
        body: Center(
          child: Column(
            mainAxisAlignment: MainAxisAlignment.center,
            children: [
              Text('Header', style: TextStyle(fontSize: 24)),
              SizedBox(height: 20),
              Container(
                padding: EdgeInsets.all(10),
                color: Colors.blue,
                child: Text('Content 1', style: TextStyle(color: Colors.white)),
              ),
              Container(
                padding: EdgeInsets.all(10),
                color: Colors.green,
                child: Text('Content 2', style: TextStyle(color: Colors.white)),
              ),
            ],
          ),
        ),
      ),
    );
  }
}
