# Сравнение micro_bench.php
Для коммита e53d922ef56f5dd540819bbf7e630c8715ed640c

## PHP 7.2.22
```
Total            408.807

empty_loop         3.665
func()            31.220    27.555
undef_func()      31.030    27.365
int_func()         8.215    4.550
$x = self::$x      7.599    3.934
self::$x = 0       7.741    4.076
isset(self::$x)    7.434    3.769
empty(self::$x)    7.763    4.098
$x = Foo::$x       8.200    4.535
Foo::$x = 0        7.564    3.899
isset(Foo::$x)     7.577    3.912
empty(Foo::$x)     7.927    4.262
self::f()         32.713    29.048
Foo::f()          33.397    29.732
$x = $this->x      7.075    3.410
$this->x = 0       7.383    3.718
$this->x += 2      7.959    4.294
++$this->x         7.694    4.029
--$this->x         7.449    3.785
$this->x++         8.419    4.754
$this->x--         8.014    4.349
isset($this->x)    6.568    2.903
empty($this->x)    6.911    3.246
$this->f()        33.305    29.640
$x = Foo::TEST     7.519    3.854
new Foo()         26.479    22.814
$x = TEST          6.591    2.926
$x = $_GET         8.507    4.842
$x = $GLOBALS['v'] 7.337    3.672
$x = $hash['v']    6.870    3.205
$x = $str[0]       7.202    3.537
$x = $a ?: null    8.463    4.798
$x = $f ?: tmp     9.509    5.844
$x = $f ? $f : $a  8.714    5.049
$x = $f ? $f : tmp 8.789    5.124
overhead 3.66498208
------------------------
Total            408.807
```

## PHP 7.4.7
```
Total             38.902
Total             37.365
Total             35.793
Total             36.158
Total             34.868

empty_loop         0.309
func()             0.846    0.537
undef_func()       1.017    0.708
int_func()         0.523    0.213
$x = self::$x      1.268    0.959
self::$x = 0       1.040    0.731
isset(self::$x)    1.275    0.966
empty(self::$x)    1.270    0.961
$x = Foo::$x       0.893    0.584
Foo::$x = 0        0.685    0.375
isset(Foo::$x)     0.887    0.578
empty(Foo::$x)     0.911    0.602
self::f()          1.214    0.905
Foo::f()           1.047    0.738
$x = $this->x      0.788    0.479
$this->x = 0       0.747    0.437
$this->x += 2      0.877    0.568
++$this->x         0.871    0.562
--$this->x         0.852    0.543
$this->x++         0.961    0.652
$this->x--         0.936    0.627
isset($this->x)    1.057    0.748
empty($this->x)    1.270    0.961
$this->f()         1.075    0.766
$x = Foo::TEST     0.821    0.512
new Foo()          2.965    2.656
$x = TEST          0.756    0.447
$x = $_GET         1.581    1.272
$x = $GLOBALS['v'] 0.655    0.346
$x = $hash['v']    1.160    0.851
$x = $str[0]       1.038    0.729
$x = $a ?: null    1.117    0.808
$x = $f ?: tmp     1.068    0.759
$x = $f ? $f : $a  1.202    0.893
$x = $f ? $f : tmp 1.175    0.866
overhead 0.30909039
------------------------
Total             36.158
```

## KPHP
```
Total              4.434
Total              4.379
Total              4.340
Total              5.068
Total              4.933

empty_loop         0.000
func()             0.000    -0.000
undef_func()       0.000    -0.000
int_func()         0.631    0.631
$x = self::$x      0.000    -0.000
self::$x = 0       0.017    0.017
isset(self::$x)    0.000    -0.000
empty(self::$x)    0.000    -0.000
$x = Foo::$x       0.000    -0.000
Foo::$x = 0        0.018    0.018
isset(Foo::$x)     0.000    -0.000
empty(Foo::$x)     0.000    -0.000
self::f()          0.000    -0.000
Foo::f()           0.000    -0.000
$x = $this->x      0.033    0.033
$this->x = 0       0.034    0.034
$this->x += 2      0.101    0.101
++$this->x         0.102    0.102
--$this->x         0.103    0.103
$this->x++         0.100    0.100
$this->x--         0.125    0.125
isset($this->x)    0.036    0.036
empty($this->x)    0.034    0.034
$this->f()         0.000    -0.000
$x = Foo::TEST     0.000    -0.000
new Foo()          1.081    1.081
$x = TEST          0.000    0.000
$x = $_GET         0.231    0.231
$x = $GLOBALS['v'] 0.000    -0.000
$x = $hash['v']    0.421    0.421
$x = $str[0]       0.437    0.437
$x = $a ?: null    0.544    0.544
$x = $f ?: tmp     0.000    0.000
$x = $f ? $f : $a  0.386    0.386
$x = $f ? $f : tmp 0.000    0.000
overhead 0.00000143
------------------------
Total              4.434
```
