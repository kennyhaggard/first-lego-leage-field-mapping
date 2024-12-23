# first-lego-leage-field-mapping
A tool to plot paths for First Lego League

Welcome! This tool is designed to help First Lego Leauge teams plan their movement across the field.

It's a simple script that relies on providing a json text file with a set of missions.

It assumes a couple of things:
1) Zero point turns at the center of the robot (likely not truly accurate as wheel bases are usually skewed towards one side of a robot)
2) Movement timing is not true to speed, it is simply about where the robot goes.
3) It does require your robot to accurately turn! This is best accomplished relying on the yaw of the hub. This can be achieved in python or block code.

Here is what a mission looks like in JSON format:
Any missions uploaded must be in this format!
[
    {
        "name": "Mission 1",
        "startX": 0,
        "startY": 0,
        "startAngle": 90,
        "robotWidthCm": 30,
        "robotHeightCm": 13,
	"traceColor": "green",
        "actions": [
            { "type": "move", "value": 17},
            { "type": "rotate", "value": -24 },
            { "type": "move", "value": 30 },
            { "type": "move", "value": -30 },
            { "type": "rotate", "value": 24 },
	    { "type": "move", "value": -17}
        ]
    },
    {
        "name": "Mission 2",
        "startX": 0,
        "startY": 30,
        "startAngle": 0,
        "robotWidthCm": 30,
        "robotHeightCm": 12,
	"traceColor":"red",
        "actions": [
            { "type": "move", "value": 50 },
            { "type": "rotate", "value": 90 },
            { "type": "move", "value": 10 }
        ]
    },
    {
        "name": "Mission 3",
        "startX": 150,
        "startY": 30,
        "startAngle": 180,
        "robotWidthCm": 10,
        "robotHeightCm": 12,
	"traceColor": "yellow",
        "actions": [
            { "type": "move", "value": 50 },
            { "type": "rotate", "value": -90 },
            { "type": "move", "value": 10 }
        ]
    },
    {
        "name": "Mission 4",
        "startX": 150,
        "startY": 30,
        "startAngle": 180,
        "robotWidthCm": 10,
        "robotHeightCm": 12,
	"traceColor":"blue",
        "actions": [
            { "type": "move", "value": 50 },
            { "type": "rotate", "value": -90 },
            { "type": "move", "value": 10 }
	]
        
    },
    {
        "name": "Mission 5",
        "startX": 150,
        "startY": 30,
        "startAngle": 180,
        "robotWidthCm": 10,
        "robotHeightCm": 12,
	"traceColor":"purple",
        "actions": [
            { "type": "move", "value": 50 },
            { "type": "rotate", "value": -90 },
            { "type": "move", "value": 10 }
	]        
    }
]

Good luck and have fun!
