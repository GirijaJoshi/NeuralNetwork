# NeuralNetwork and Deep learning
This challenges check the use of different NeuralNetwork and Deep learning techiniques to check the performace of the model. We are using charity_data.csv file.
### Analysis
Pandas is used to read the charity_data.csv file. By looking at the file there were may columns with type object. 
* First by looking at the description provided in the module challenge there are two columsn EIN and NAME which are not usful to findout the success of the load application aprroval. So we have removed those columns from the input features.
* I have used funnel shape neurons for this model. First layer started with number of neurons same as number of inputs and send layer is half of the number of neurons as first layer and outout layer has one as it is clraffication either 0 or 1 of application successful or not
* First try was using relu model with 2 layers and output layer. As relu is most widely used funtion, here we can back-propagate the errors and have multiple layers of neurons being activated by the ReLU function, it does not activate all the neurons at the same time.
* Steps taken to improve model peformace:
    * Removed unnesessary features from input.
    * Couple of inputs had value count with large number of variation. Using value count foundout the range and kept only those inputs with large value in its own bucket and rest put it in 'Other' bucket.
    * Used funnel shaped number of neurons.
    * Used Dropout functionality.
    * Also kept only those application which are active.
    * Tried different combination of activation function and number of hidden layers.
* Tried different combination od neural netowrk and deep learning and came to conclusion with this data accuracy of test data does not change very much. So there is no strong recomendation but relu behaves little better.

