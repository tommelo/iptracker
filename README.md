# iptracker
IP Location Tracker

```
                                      Hey there!
                                    186.231.139.85
                                     is that you?
                                        /
   _______________          _______________
  |  ___________  |        |  ___________  |
  | |           | |        | |           | |
  | |   X   X   | |        | |           | |
  | |     -     | |        | |   0   0   | |
  | |    ___    | |        | |     -     | |
  | |   /   \   | |        | |   \___/   | |
  | |   \___/   | |        | |           | |
  | |___________| |        | |___________| |
  |_______________|        |_______________|
    ____|   |___.............._|________|_
   | ********** |            | ********** |
   | ********** |            | ********** |
    ------------              ------------
```

##Dependencies
```
pip install pygeoip
```


###Options
```
-v --version shows the current version
-t --target  the target host
-h --help    shows the help usage

```

###Usage
```
python iptracker.py -t target.com
```

###Example
```
python iptracker.py -t google.com

{
    "area_code": 650, 
    "city": "Mountain View", 
    "continent": "NA", 
    "country_code": "US", 
    "country_code3": "USA", 
    "country_name": "United States", 
    "dma_code": 807, 
    "latitude": 37.41919999999999, 
    "longitude": -122.0574, 
    "metro_code": "San Francisco, CA", 
    "postal_code": "94043", 
    "region_code": "CA", 
    "time_zone": "America/Los_Angeles"
}
```

```
python iptracker.py -t 186.231.139.89

{
    "area_code": 0, 
    "city": "São Paulo", 
    "continent": "SA", 
    "country_code": "BR", 
    "country_code3": "BRA", 
    "country_name": "Brazil", 
    "dma_code": 0, 
    "latitude": -23.473299999999995, 
    "longitude": -46.66579999999999, 
    "metro_code": null, 
    "postal_code": null, 
    "region_code": "27", 
    "time_zone": "America/Sao_Paulo"
}
```
