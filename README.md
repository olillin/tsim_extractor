<div> 
    <h1 align="center">TSim Extractor</h2>
    <p align="center" style="font-style: italic;"> 
        A python script. It extracts sensor and switch positions from 
        <span style="font-weight: bold;">TSim .map</span> files and converts them to Java source code. TSim is used in the course 
        <span style="font-weight: bold;">Principles of Concurrent Programming</span>
        (TDA384 / DIT392) at Chalmers University of Technology and University of Gothenburg.
    <p>
    <p align="center">made by <a href="https://github.com/Toireosu">William Lindgren / Duplo</a><p>
</div>

## How To

```
usage: tsim_extractor [-h] [--output_file OUTPUT_FILE] [--sensor_name SENSOR_NAME] [--switch_name SWITCH_NAME] [--sensor_list_name SENSOR_LIST_NAME] [--switch_list_name SWITCH_LIST_NAME]
                      [--list_push_name LIST_PUSH_NAME] [-V]
                      INPUT_FILE

Converts a TSim map to Java source code.

positional arguments:
  INPUT_FILE            tsim map data input file

options:
  -h, --help            show this help message and exit
  --output_file OUTPUT_FILE
                        output .java file to write to
  --sensor_name SENSOR_NAME
                        name in Java file for sensor class
  --switch_name SWITCH_NAME
                        name in Java file for switch class
  --sensor_list_name SENSOR_LIST_NAME
                        name in Java file for sensor list
  --switch_list_name SWITCH_LIST_NAME
                        name in Java file for switch list
  --list_push_name LIST_PUSH_NAME
                        name in Java file for 'push'/'append'/'add' function on list
  -V, --version         show program's version number and exit
```

The script is written in Python and can be run as such:\
```
python tsim_extractor.py "some.map"
```

There is also a wrapper for __Windows__ (tsim_extractor.bat) as well as __Unix__ (tsim_extractor.sh).

## License

MIT-license. See ```LICENSE```.