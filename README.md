MTKPower hint parser for pixel-libperfmgr
===========

Usage
----------
```
python3 main.py refs/powerscntbl.xml refs/powerhint.json
```

Reference configurations
------------------------
These configurations are based uppon MT6877 platform (MediaTek Dimensity 1080)

[powerscntbl.xml](refs/powerscntbl.xml)

[powerhint.json](refs/powerhint.json)


Example output
--------------
```
[ROUND] [LAUNCH] CPULittleClusterMinFreq: 3000000 -> 2000000
[ROUND] [LAUNCH] CPUBigClusterMinFreq: 3000000 -> 2600000
[ROUND] [AUDIO_STREAMING_LOW_LATENCY] CPULittleClusterMinFreq: 1500000 -> 1503000
[ROUND] [AUDIO_STREAMING_LOW_LATENCY] CPUBigClusterMinFreq: 1000000 -> 1040000
[ROUND] [INTERACTION] CPULittleClusterMinFreq: 1075000 -> 1150000
[ROUND] [INTERACTION] CPULittleClusterMaxFreq: 3000000 -> 2000000
[ROUND] [INTERACTION] CPUBigClusterMaxFreq: 3000000 -> 2600000
{
  "Actions": [
    {
      "PowerHint": "LAUNCH",
      "Node": "CPULittleClusterMinFreq",
      "Duration": 0,
      "Value": "2000000"
    },
    {
      "PowerHint": "LAUNCH",
      "Node": "CPUBigClusterMinFreq",
      "Duration": 0,
      "Value": "2600000"
    },
    {
      "PowerHint": "LAUNCH",
      "Node": "DRAMOppMin",
      "Duration": 0,
      "Value": "1"
    },
    {
      "PowerHint": "LAUNCH",
      "Node": "TAUclampMin",
      "Duration": 0,
      "Value": "100"
    },
    {
      "PowerHint": "AUDIO_STREAMING_LOW_LATENCY",
      "Node": "CPULittleClusterMinFreq",
      "Duration": 0,
      "Value": "1503000"
    },
    {
      "PowerHint": "AUDIO_STREAMING_LOW_LATENCY",
      "Node": "CPUBigClusterMinFreq",
      "Duration": 0,
      "Value": "1040000"
    },
    {
      "PowerHint": "INTERACTION",
      "Node": "CPULittleClusterMinFreq",
      "Duration": 0,
      "Value": "1150000"
    },
    {
      "PowerHint": "INTERACTION",
      "Node": "CPUBigClusterMinFreq",
      "Duration": 0,
      "Value": "1140000"
    },
    {
      "PowerHint": "INTERACTION",
      "Node": "CPULittleClusterMaxFreq",
      "Duration": 0,
      "Value": "2000000"
    },
    {
      "PowerHint": "INTERACTION",
      "Node": "CPUBigClusterMaxFreq",
      "Duration": 0,
      "Value": "2600000"
    },
    {
      "PowerHint": "INTERACTION",
      "Node": "TAUclampMin",
      "Duration": 0,
      "Value": "40"
    }
  ]
}
```
