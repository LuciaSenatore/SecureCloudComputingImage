# Directory Content

## **ProgettoNN1.ipynb**
This notebook includes:
- The generation of the test set used to evaluate the networks (Section _1_).
- The evaluation of the NN1 network's accuracy (Section _2_) on the clean test set.
- The generation of attacks using the ART library in both generic error and specific error versions (Section _3_). Each attack was generated by varying its characteristic parameters.
- The evaluation of NN1 against the generated adversarial examples (Section _3_), including the generation of SECs and curves representing the perturbation variation based on the selected parameters.

## **ProgettoNN2.ipynb**
This notebook includes:
- The evaluation of the NN2 network's accuracy (Section _4_) on the clean test set.
- The evaluation of the transferability of each attack on NN2 (Section _5_).
- The generation of SECs.

## **ProgettoDetector.ipynb**
This notebook includes the implementation of the chosen defense mechanism and its performance against various attacks.

## **SEC File Folders**

# Running the Code
To run **ProgettoNN1.ipynb** and **ProgettoDetector.ipynb**, you'll need to create a Conda environment. You can do so by executing the following commands:

```
conda create --name ARTEnv python=3.9.19
```

```
conda activate ARTEnv
```

```
pip install torch==2.2.2 torchvision==0.17.2 adversarial-robustness-toolbox==1.18.1 facenet-pytorch==2.6.0 matplotlib==3.9.2 tensorflow==2.17.0
```

After configuring the environment, you can run the code within the notebooks to generate attacks, evaluate the model on the clean and adversarial test sets, and train the adversarial example detector.

To run **ProgettoNN2.ipynb**, copy the **python37** folder into your local Anaconda environments directory. Then, activate the environment using Anaconda Prompt with the following command:

```
conda activate python37
```

After configuring the environment, you can run the notebook to evaluate the NN2 model's performance on the clean test set and adversarial examples.