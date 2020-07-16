# Moment Steps

This step allows you to change times to a more readable format. It uses the [moment.js](https://momentjs.com) library.


---------

<kbd>
<a href="https://support.xmatters.com/hc/en-us/community/topics">
   <img src="https://github.com/xmatters/xMatters-Labs/raw/master/media/disclaimer.png">
</a>
</kbd>

---------

# Files

* [MomentSteps.zip](MomentSteps.zip) - Workflow zip file with the step and example flow
* [moment.png](/moment.png) - Moment logo

# How it works
Moment.js accepts a wide variety of formats for a date and time. On top of this, the step includes an input called **epoch?**. It helps support formats like unix, ms, microseconds, ns. All these can be used for the input to change how the date is created.


# Installation

## xMatters Setup
1. Download the [MomentSteps.zip](MomentSteps.zip) file onto your local computer
2. Navigate to the Workflows tab of your xMatters instance
3. Click Import, and select the zip file you just downloaded


## Usage

### Inputs
| Name  | Required? | Min | Max | Help Text | Default Value | Multiline |
| ----- | ----------| --- | --- | --------- | ------------- | --------- |
| Date/Time | Yes | 0 | 2000 | Date and time. Can be in many formats. Anything the moment.js library can accept. https://momentjs.com | | No |
| Output Timezone | Yes | 0 | 2000 | Timezone for output date/time. Formatted like America/New_York | | No |
| epoch? | Yes | 0 | 2000 | This is if the value has to do with time since epoch. Can be seconds (true), milliseconds, microseconds, or nanoseconds | false | No |
| Output Format | No | 0 | 2000 | Format of the output. For more info on this: https://momentjs.com/docs/#/parsing/string-format/ |  | No |


### Outputs

| Name | Description |
| ---- | ----------  |
| formattedDate | The date formatted in Moment |


## Example
This is what the included flow looks like.

<kbd>
	<img src="/media/ExampleFlow.png">
</kbd>

