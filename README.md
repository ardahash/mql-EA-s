# mql-EA-s

compilation of EA's I wrote to learn MQL4 language. Doing this to automate leveraged cryptocurrency trading in ByBit.

testing and optimization: in MT4 you can not perform walk-forward modeling and optimization directly. I have researched the easiest way to do this manually is just to split the training/testing data in half. For example: in MT5 you can select a full date range and just perform walk-forward. in MT4 you need to split the date into 2 equal partitions, you need to optimize the EA properties for the first data partition, and model the results on the second partition. Make sure partitions are not split at a day (dont make 1 partition end on monday, and other start on monday. you need to end 1 on monday and start the next one on tuesday in order to avoid data overlap) otherwise the data creates a biased profitable model. 
