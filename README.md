# Stack RNN
Stack RNN is a project gathering the code from the paper 
*Inferring Algorithmic Patterns with Stack-Augmented Recurrent Nets* by Armand Joulin and Tomas Mikolov.

Most of the experiments shown in the paper can be reproduced by running the script `script_tasks.sh`.

We also include the code to reproduce the experiement on language modeling.

## Examples
To run the code on a task:
```
make toy
> ./train_toy  -ntask 1 -nchar 2 -nhid 10 -nstack 1 -lr .1 -nmax 10 -depth 2 -bptt 50 -mod 1
```
To run the code on language modeling:
```
> make word
> ./train_word -nhid 40 -nstack 10 -mod 2 -bptt 50 -lr .1 -depth 1
```
Note that you need to put the Penn Trebank data in the data folder.

## Requirements
Stack RNN works:
* Mac OS X
* Linux

It was not tested on Windows. 
To compile the code a relatively recent version of g++ is required.

## Building Stack RNN
Run `make` to compile everything. 


## Options
For more help about the options:
```
> make toy
> ./train_toy --help
```



## Join the Stack RNN community
* Paper: http://arxiv.org/abs/1503.01007
* Facebook page: https://www.facebook.com/fair
* Contact: ajoulin@fb.com
See the CONTRIBUTING file for how to help out.

## License
Stack RNN is BSD-licensed. We also provide an additional patent grant




