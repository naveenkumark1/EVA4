# Assignment

## 1) What are Channels and Kernels ?

Channel : It is a layer with collection of similar type of features

Kernel : Kernel is a filter that is used to extrac particular feature from the channel

## Why should we (nearly) always use 3x3 kernels?

3X3 is best to extract the features with less number of features, 

Keeping in mind the processing power requried to process 5X5, 3X3 captures better features with optimum processing power.

## How many times to we need to perform 3x3 convolutions operations to reach close to 1x1 from 199x199 (type each layer output like 199x199 > 197x197...)

99 Times

	Reduction due to convolution 		199
--	2	->	197
--	2	->	195
--	2	->	193
--	2	->	191
--	2	->	189
--	2	->	187
--	2	->	185
--	2	->	183
--	2	->	181
--	2	->	179
--	2	->	177
--	2	->	175
--	2	->	173
--	2	->	171
--	2	->	169
--	2	->	167
--	2	->	165
--	2	->	163
--	2	->	161
--	2	->	159
--	2	->	157
--	2	->	155
--	2	->	153
--	2	->	151
--	2	->	149
--	2	->	147
--	2	->	145
--	2	->	143
--	2	->	141
--	2	->	139
--	2	->	137
--	2	->	135
--	2	->	133
--	2	->	131
--	2	->	129
--	2	->	127
--	2	->	125
--	2	->	123
--	2	->	121
--	2	->	119
--	2	->	117
--	2	->	115
--	2	->	113
--	2	->	111
--	2	->	109
--	2	->	107
--	2	->	105
--	2	->	103
--	2	->	101
--	2	->	99
--	2	->	97
--	2	->	95
--	2	->	93
--	2	->	91
--	2	->	89
--	2	->	87
--	2	->	85
--	2	->	83
--	2	->	81
--	2	->	79
--	2	->	77
--	2	->	75
--	2	->	73
--	2	->	71
--	2	->	69
--	2	->	67
--	2	->	65
--	2	->	63
--	2	->	61
--	2	->	59
--	2	->	57
--	2	->	55
--	2	->	53
--	2	->	51
--	2	->	49
--	2	->	47
--	2	->	45
--	2	->	43
--	2	->	41
--	2	->	39
--	2	->	37
--	2	->	35
--	2	->	33
--	2	->	31
--	2	->	29
--	2	->	27
--	2	->	25
--	2	->	23
--	2	->	21
--	2	->	19
--	2	->	17
--	2	->	15
--	2	->	13
--	2	->	11
--	2	->	9
--	2	->	7
--	2	->	5
--	2	->	3
--	2	->	1

## How are kernels initialized? 

Kernals are initialsed randomly with random weights

## What happens during the training of a DNN?

During the trinaing of the DNN two stages will be there, 

## Feed forward: 
In this stage the randomy initialsised weights combine with the activation functions and gives an output. 
The output is compared with the actual output and the error is measured, The error is sent back in to the network as feedback.

## Feedback : 
In this stage the error which is sent back in to the network alters the randomly initiated weights as per some predefined quantity ( Learning rate )

These two stages happen to and fro several times ( This cycle is called epoch ) untill the output of the network is almost equal to the expected output. 
