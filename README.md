# week6flutter

import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'My Simple App',
      home: Scaffold(
        appBar: AppBar(
          title: Text('My Simple App'),
        ),
        body: Center(
          child: Column(
            mainAxisAlignment: MainAxisAlignment.center,
            children: <Widget>[
              Text(
                'Welcome to My App!',
                style: TextStyle(fontSize: 24),
              ),
              SizedBox(height: 20), // Space between widgets
              ElevatedButton(
                onPressed: () {
                  print('Button clicked!');
                },
                child: Text('Click Me'),
              ),
              SizedBox(height: 20), // Space between widgets
              Image.network(
                'https://via.placeholder.com/150', // Example image URL
                width: 150,
                height: 150,
              ),
            ],
          ),
        ),
      ),
    );
  }
}
