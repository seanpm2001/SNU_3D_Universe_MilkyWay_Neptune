name: Makefile CI

on:
  push:
    branches: [ "SNU_3D_Universe_MilkyWay_Neptune_Main-dev" ]
  pull_request:
    branches: [ "SNU_3D_Universe_MilkyWay_Neptune_Main-dev" ]

jobs:
  build:

    runs-on: ubuntu-latest

    steps:
    - uses: actions/checkout@v3

    - name: configure
      run: ./configure

    - name: Install dependencies
      run: make

    - name: Run check
      run: make check

    - name: Run distcheck
      run: make distcheck
