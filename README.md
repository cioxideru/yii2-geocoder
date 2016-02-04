# yii2-geocoder

Installation
============

This document will guide you through the process of installing Yii2-geocoder using **composer**.

Download Yii2-geocoder using composer
-----------------------------------------

Add `"deka6pb/yii2-geocoder": "*"` to the require section of your **composer.json** file and run
`composer update` to download and install Yii2-autoparser.

Methods:

```
findByAddress($address, array $params = [], $results = 10)

findOneByAddress($address, array $params = [])

findByPoint(Point $point, $kind, Point $radius = null, array $params = [], $results = 10)

findByOnePoint(Point $point, $kind, Point $radius = null, array $params = [])
```

For example:

```
$address = "2707 Congress St., San Diego, CA 92110";

/* @var CoderInterface $coder */
$coder = Geocoder::build(Geocoder::TYPE_GOOGLE);
$object = $coder::findOneByAddress($address);
```
