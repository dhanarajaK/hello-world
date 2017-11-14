[![Datmo Model](https://datmo.com/datmo/hello-world/badge.svg)](https://datmo.com/datmo/hello-world)

# Hello World

This is an example of a Datmo Model which uses iris dataset to classify between different flower types. This project tries nearest neighbor and naive bayes algorithms. 

The Iris dataset was used in R.A. Fisher's classic 1936 paper and can also be found on the [UCI Machine Learning Repository][1] and is a classic hello world dataset and problem for machine learning. 

It includes three iris species with 50 samples each as well as some properties about each flower. One flower species is linearly separable from the other two, but the other two are not linearly separable from each other.

The columns in this dataset are:

 - Id
 - SepalLengthCm
 - SepalWidthCm
 - PetalLengthCm
 - PetalWidthCm
 - Species

  [1]: http://archive.ics.uci.edu/ml/

Check out the Snapshots tab on Datmo above for information on snapshots that were taken with various parameters. Search and filter them to find the best ones.

Clone this model on your local machine with the Datmo CLI

     $ datmo clone hello-world

Now you can run the set of commands below to better understand the advantages of converting a repository to a Datmo Project. First you can check out all of the snapshots that have already been created by the user.

     $ datmo snapshot ls 

Once you have viewed all of the existing snapshots, you can create your own by simply running the code below which runs the classification training which saves a few key files (the weights file, metrics for this file) in the output directory which creates a new snapshot.

     $ datmo task run "python3 classifier.py"

For reference, here are few more quick details about what you can find in the repository.

Dockerfile: this is meant to keep track of your environment. For example, this Dockerfile ensures that our environment has all of the requirements needed to run our model. You can manage, edit, and create new enviroments with the [datmo env command](https://docs.datmo.com/commands/environment.html).  You can learn more about environments with Docker on our [Datmo docs page](https://docs.datmo.com/guides/creating-your-environment.html)

Happy Building :)
