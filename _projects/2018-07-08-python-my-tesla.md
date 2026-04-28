---
title: "Tesla Python API"
excerpt: "Python library to control Tesla vehicles"
header:
  teaser: /assets/images/projects/python-my-tesla.jpg
sidebar:
  - title: "Repository"
    text: "[![GitHub stars](https://img.shields.io/github/stars/zmsp/python-my-tesla?style=for-the-badge)](https://github.com/zmsp/python-my-tesla/stargazers)  \n[![GitHub forks](https://img.shields.io/github/forks/zmsp/python-my-tesla?style=for-the-badge)](https://github.com/zmsp/python-my-tesla)"
toc: true
categories:
  - software
tags:
  - API
  - python
---

A Python library designed to allow users to easily interface with the Tesla API and control their vehicles programmatically.

## The Story

I was excited to create a Tesla Python library that would allow others to easily interface with the Tesla API. Finally, I released the library to the public and it was an instant hit! People were able to use it to do all sorts of things.

### Community Coverage
- [I hacked my Tesla - it turned out to be a bad idea](https://mikesml.com/2021/01/30/i-hacked-my-tesla-it-turned-out-to-be-a-bad-idea/)
- [Can I control my Tesla with a Python program?](https://medium.com/@Dei8ht/can-i-control-my-tesla-with-a-python-program-83e3e115af40)

## Links

- **Source Code**: [GitHub Repository](https://github.com/zmsp/python-my-tesla)
- **PyPI Package**: [mytesla](https://pypi.org/project/mytesla)

## Stats (as of release)
- **Total downloads**: 9,197
- **Monthly downloads**: 217

## Documentation

### Installation
```bash
pip3 install myTesla
```

### Usage
```python
import myTesla

my_model_s = myTesla.connect('test@example.com', 'MySecurePassword')
charge_state = my_model_s.charge_state()
door_lock = my_model_s.door_lock()
my_model_s.honk_horn()

print(charge_state)
print(door_lock)
```

## Legal Disclaimer

This program is provided as is. This program is not supported or endorsed by Tesla Motors. By using this software, you agree to not hold the author (Zobair Shahadat) and any of the contributors liable for anything.