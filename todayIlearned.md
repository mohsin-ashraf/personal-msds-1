# Today I Learned (TIL)

Caution: This timeline is tailored for **@mohsin-ashraf** and might not be suitable for everyone. 

After completing this challenge I will complete [this](https://triplebyte.com/candidates/tracks) quiz and plan for [this](https://www.deeplearning.ai/) quiz to have a proof of my skills.


## Day 100 | July 14 2020 | Tuesday
Today I completed the Amazon SageMaker Deep dive video course by going through with all the available videos at this point of time. And also completed my ***100 days of MSDS!***
- Amazon SageMaker Ground Truth.
	- Build highly accurate training data using machine learning and reduce the labeling costs by up to 70%.
		- Amazon Machanical Turk workers.
		- Private labeling workforce.
		- Third-Party vendors.
		- Built in data labeling tasks.
			- Bounding boxes.
			- Image Classification.
			- Semantic Segmentation.
			- Text Classification.
			- Named Entity Recognition.
		- Features of amazon labeling tasks.

## Day 99 | July 13 2020 | Monday
Today I continued with the Amazon SageMeker Deep dive and learned about using deep learning frameworks of your choice, feature engineering and Schdule predictions.
- Using deep learning framework of your choice.
	- Using the script mode.
		- Managed Docker container.
		- Put the python script in the container.
	- Using the sci-kit learn for training job.
		- Set the `train_instance_type` to `local`.
		- Don't use the `sagemaker_session`.
- Co-relation analysis of dataset using feature engineering with Amazon SageMaker.
- Batch Transforms.
- For the best outcome use the pre-built examples on SageMaker and change it according to your requirements.

## Day 98 | July 12 2020 | Sunday
Today I continued with the Amazon SageMaker Deep dive and learned about Training the ML models, Deploying the model, hyperparameter optimization and scaling up the model training.
- Train your ML models.
	- Each sageMaker notebook instance has its own **ephemeral cluster** of a single EC2 instance or sometimes multiple.
	- This EC2 instance is alive for the number of seconds your model is alive.
	- This cluster is gonna comes down after it finishes its training.
	- Configurations for Model training.
	- Model evaluation.
	- Hyperparameter optimization.
	- Monitoring the model.
	- Checking the logs.
- Deploying the model.
	- SageMaker endpoints.
		- SageMaker automatecally creates the rest API.
- Tuning Hyperparamters in SageMaker.
	- Transfer learning.
- Scaling up training using distributed training.
	- Multiple nodes for training.
		- Master image which is passing data and code to the rest of those nodes.
	- Distributing training on single node using multiple vCPUs.
	- Fully Replicated.
		- Each node in the cluster will get the full replicated version of the original data.
	- Sharded by S3 Key.	
		- Splitting up the original dataset into multiple smaller datasets for training on multiple EC2 instances.
	- Use the already available examples and modify it according your needs.

## Day 97 | July 11 2020 | Saturday
Today I started Amazon SageMaker Deep dive for learning about amazon sageMaker jupyter notebook plateform.
- Amazon SageMaker is a fully maneged machine learning service.
	- Notebook instances.
		- These notebooks run on manged EC2 instances, which means you won't see any EC2 instance on EC2 console.
		- EC2 instance family types.
			- {t,m,c,p}
			- The latest version of an EC2 instance is always gonna be the cost efficient.
		- Adding EBS volumns (again its fully managed).
	- You can add github repository aswell.
- Built-in Machine learning algorithms with Amazon SageMaker.
	- Classifiers and Regressors.
	- Computer Vision.
	- Natural Language Processing.
	- Other machine learning algorithms.
	- All these algorithms live in a Docker container.
	- Available documentation for the algorithms and white papers.
	- **Algorithms assume the last column of your dataset is the target column.**
- Bringing your own custom model.
	- Bringing your model using Scrip mode.
		- Choose the AWS-managed container(Docker) of your choice (from available options.)
		- Write your model as a bundle of files (or it could be a single file).
		- Specify the entry point in the SageMaker Estimator.
		- Include any extra libraries with **requirements.txt**
		- Use the AWS webserver for inference.
	- Docker Container.
		- Bring your own docker container.
		- Register it in ECR.
	- AWS ML Marketplace.
		- There 230+ solutions available on Machine Learning Market place.

## Day 96 | July 10 2020 | Friday
Today I completed the course and started learning about the following topics.
- `cat` command.
	- `cat file.txt` print outs the content of the file.
	- `cat >> file.txt` prompt for adding text into the file without overriding i.e append at the end of the file.
	- `cat file1.txt file2.txt file3.txt` prints out the content of multiple files.
- `more file_name.extension` prints the content of the file for few lines and stop for the prompt.
- `less file_name.extension` is more advanced way of `more`.
- The NANO text editor.
- `sudo` commands for super user commands.
- Switching to super using using `sudo su`
- Killing process using `Ctrl + c`
- `killall servicename` kills all the running instance of the `servicename`
- Shortcuts commands in bast
	- `Ctrl + d` for logging out of terminal or in other programs.
	- `Ctrl + l` clears the terminal screen.
	- `Ctrl +` zoom in & `Ctrl + -` zoom out.
	- `Ctrl + x` followed by `backspace` removes the all the previous line in terminal.
	- Other shortcuts using `Alt` Key.
	- Cutting and pasting.
- Writing Bash Scripts.
	- `#!/bin/bash` at the top of the script.
	- comments are done using `#`
	- Variables and Arithmetic operations.
	- String manipulation.
	- while, until and for loop.
	- User input.
	- If else statements. 
	- Crontab

## Day 95 | July 9 2020 | Thursday
Today I started a new course on [Bash Scripting, Linux and Shell Programming Complete Guide](https://www.udemy.com/course/bash-scripting-course/), and started learning about the basics of bash scripting.
- `ls` command and its flags.
	- Using different flags for information purposes.
	- Regex search using `ls`.
- Printing current working directory using `pwd`
- Changing the working directory.
	- `cd -` will move you to your last directory where you were working previously.
- Checking the file type.
	- `file path_to_file`
- Looking for something in the dicrectory.
	- `locate anything` will find all the files/folders in your system which have `anything` in their name.
	- You can specify the subset directory to look at by using `grep` command. 
- Check where these commands have been stored.
	- `which ls` will show you where the `ls` command is written.
- History of the previous commands.
	- `history` 
- Getting Help.
	- `whatis command_name` will tell you what the command do replace `command_name` with some valid command for example `ls`.
	- Printing manuals for the command.
		- `man command_name` where `command_name` is any command for example `ls`
- Making folders using terminal.
	- `mkdir folder_name` will create the folder named `folder_name`.
- Creating files using `touch`.
	- `touch file_name.extension` file with name `file_name.extension` will be created.
- Coping files using `cp`.
- Moving files with `mv`.
- Deleting files and folders using `rm` and `rm -r`
- Changing file permissions.
	- Premission codes for read (4), write (2) and execution (1)
	- `chmod permission_code` will set the permission of the file according to the code.
	- [Important link](https://www.guru99.com/file-permissions.html)

## Day 94 | July 8 2020 | Wednesday
Today I started next module of the course and started learning about Neural Style Transfer and activation maps and Completed the course.
- Transforming one image with the style of another image.
- Theory behind Neural Style Transformation.
	- Gram Matrix.
		- A matrix product of input and its transpose devided by number of elements.
			- G = 1/N * X.X<sup>T</sup>
- Class Activation map.
- [Code base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-094)


## Day 93 | July 7 2020 | Tuesday
Today I started the next module of the course on object detection and learned about the Single Shot Multibox Detector(SSD) model.
- Motivation for SSD.
	- High speed and more accurate algorithm.
- Object Localization.
	- outputing the position of the object with prediction as well.
- Sliding window concept.
- Converting dense layers into convolution layers of size 1.
- Using multiple boxes of different shapes.
- [Pretrained Computer Vision Models](https://github.com/tensorflow/models/tree/master/research)
- Intersection over union. 


## Day 92 | July 6 2020 | Monday
Today I started the next module of the course and learned about the ResNet and Inception model.
- ResNet Architecture.
- Inception Model Architecture.
- Handling different sizes of the input images.
	- GlobalPooling layers.
	- [ResNet Important article](https://towardsdatascience.com/building-a-resnet-in-keras-e8f1322a49ba)
	- [ResNet Important article](https://towardsdatascience.com/understanding-and-coding-a-resnet-in-keras-446d7ff84d33)
		- [Implement ResNet by yourself](https://github.com/priya-dwivedi/Deep-Learning/tree/master/resnet_keras)
- [Other computer vision models](https://machinelearningmastery.com/how-to-use-transfer-learning-when-developing-convolutional-neural-network-models/)

## Day 91 | July 5 2020 | Sunday
Today I started a course on [Deep Learning: Advanced Computer Vision](https://www.udemy.com/course/advanced-computer-vision/) a practical course on computer vision applications.
- Basic Overview of the Convolutional Neural Network.
- Transfer learning.
- Visual Geometery Group (VGG) Network.
	- Arcitecture of VGG.
	- You can change the last layer of the VGG depending upon the use case you are working for.
	- Using VGG16 for dogs-cats classification.
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-091)

## Day 90 | July 4 2020 | Saturday
Today I completed the next course by learning about Vanishing Gradients and Dimentionality reduction applications in NLP.
- Vanishing Gradients.
	- When you have a deep neural network, gradients get smaller and smaller the further back you go.
	- When you multiply a small number (< 1) with another samll number the number become even smaller.
- Applications to NLP.
	- Latent Semantic Analysis (LSA).
- Applications to Recommender Systems.
	- Data representation for Recommendation systems.
		- One hot encoding for this type of problem is not suitable, since there are going to be millions of users and thousands of movies.
	- Autoencoders compressed representation of the input data.
		- Autoencoders learn vectors who represent the users and their features regarding the problem (in this case he likes action or horror movies etc).
		- Autoencoders can also be used to recommend movies, as for reconstructing the data of the users. That is, all the movies which the user hasn't yet watched has not rating (consider no rating = noise), Our auto-encoder can reconstruct the rating for the movies that the user hasn't yet rated.
		- You might need to write your own cost function. 
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-090).

## Day 89 | July 3 2020 | Friday
Today I started learning about the Auto-Encoders a deep learning method for dimentionality reduction and finding the latent spaces.
- [Autoencoders](https://towardsdatascience.com/auto-encoder-what-is-it-and-what-is-it-used-for-part-1-3e5c6f017726)
	- Is an unsupervised artificial neural network that learns how to efficiently compress and encode data then learns how to reconstruct the data back from the reduced encoded representation to a representation that is as close to the original input as possible.
	- Components of the Autoencoders.
		- Encoder.
		- Bottleneck
		- Decoder.
		- Reconstruction loss.
	- Cross entropy loss function.
	- Autoencoders for data visualization.
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-089).	


## Day 88 | July 2 2020 | Thursday
Today I start a new course on [Unsupervised Deep Learning in Python](https://www.udemy.com/course/unsupervised-deep-learning-in-python/) and learned the following topics.
- Principle Component Analysis (PCA).
	- An algorithm which reduces the dimentionality of the data by capturing the correlation between multiple variables and comimg with with lower number of variables to repsent the data.
	- Finding vectors in the lower dimentions such that there is no correlation between the vectors of the PCA.
	- Direction of the component vector is the same where the maximum variance of the data is.
	- Select only those component vectors from PCA that explain the high variance, and leave the component vectors which just explains the noise.
	- Large variations in the dataset are considered as signals and tiny tiny variations are considered as noise.
- Derivation of PCA.
	- Covariance Matrix for input features = Matrix<sub>x</sub> = 1/N (X- mean(X))<sup>T</sup>(X - mean(X))
	- Eigen decomposition of covariance matrix.
- PCA only ratates the data.
	- Multiplying by the PCA matrix changes only its direction.
- PCA Example.
- PCA Implementation.
- Application of PCA using Naive Bayes.
	- PCA gives orthoganal vectors.
	- Naive Bayes Classifier assumes the features are independent of each others.
- Singular Value Decomposition (SVD).
- Its a non-linear method hence its more expressive than PCA.
- There is no transform function for t-SNE.
	- t-SNE modifies the outputs of directly in order to minimize the cost function.
- Gaussion Clouds and t-SNE.
- t-SNE with MNIST
- t-SNE with XOR
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-088)

## Day 87 | July 1 2020 | Wednesday
Today I completed the course on Feature Engineering for Machine Learning and wrapped up its last couple of sections and learned the following topics.
- Engineering mixed variables.
	- Creating saperate features for each type of the variable (labes and integers in the column can be expanded into multiple columsn containing only labels and integers).
	- Splitting the Mixed variables into meaningful features. For example PK-177 can be splitted in PK for pakistan and 177 for flight number.
- Engineering Datetime variables.
	- Simple Using Months days or Years.
	- Time periods
- Assembling a feature engineering pipeline.
	- Building a complete end to end machine learning pipeline from loading data to saving model and benchmarking.
	- Using different functions for different variables for cleaning and scaling.
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-087)


## Day 86 | June 30 2020 | Tuesday
Today I started the next modules of the course on Outlier Handling and Feature Scaling. Following are the topics that I learned.
- Outlier Handling.
	- An outlier is a data point which is significantly different from the remaining data.
	- Some of the possible ways to handle outliers.
		- Removing outliers from the dataset.
		- Treat outliers as missing data and perform missing data imputation.
		- Capping top/bottom of the variable.
		- Using Quantiles to remove values from above and below of that quantile.
- Feature Scaling.
	- Refers to the methods used to normalize the range of values of independent variables.
	- Standardisation.
		- Centers the variable at 0 and sets the variance to 1.
		- formula = (X - mean(X)) / Std(X).
		- Preserves the shape of the original distribution.
	- Mean Normalization.
		- Centers the variable at 0 and re-scales the variable to the value range.
		- formula = (X - mean(X))/(max(X) - min(X))  :. range = max(X) - min(X)
	- MinMax Scaling.
	- Maximum Absolute Scaling.
		- X / max(X)
		- Scales the variable upto 1.
	- Robust Scaling. 
	- Scaling to unit norm.
[Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-086) 


## Day 85 | June 29 2020 | Monday
Today I continued with the course and moved on to learn more techniques of feature engineering explored the following topcis.
- Variable transformations.
	- Transformation of the variables such that they follow the desired distribution.
	- Different Transformation functions available for transform the variables.
	- Gaussian Transformation.
	- Scikit-learn Transformers.
		- FunctionTransformer takes in transformation function and variable to transform.
- Discretisation.
	- Transforming a continous variable to a categorical variable using bins.
	- Equal Width Discretisation.
		- Devides the variable values into N bins of the same width.
		- width = (max(variable) - min(variable)) / N
	- Equal frequency discretisation.
		- Divides the values of the variable into N bins, such that each bin carries the same number of observations.
	- K-Means Discretisation.
		- This discretisation method consists in applying K-Means clustering to the continous variable.
	- Discretisation and categorical encoding.
		- Can convert the bins of the discretisation into categories and then apply categorical variable encoding.
	- Discretisation using decision trees.
	- Using Domain knowledge for descritisation.
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-085)


## Day 84 | June 28 2020 | Sunday
Today I continued with the same course and moved on to the next modules of the course categorical variable encoding.
- Categorical variable encoding refers to converting the categorical values to some numerical representation.
- One hot encoding.
	- K values of a categorical feature can be converted to K -1 one hot encoding. 
	- Using Training data for the one-hot-encoder to train and transform it for test data, you might wanna ignore not seen labels in training set when they appear in the test set.
	- Feature space can expand.
- One hot encoding of top categories.
	- Performing one hot encoding, only considering the top n most frequent categories.
	-  Feature space is can be limited.
- Ordinal Encoding.
	- Replacing the categorical values with integers from 1 to n.
- Count/Frequency Encoding
	- Categorical values are replaced by the number of times they appear or with the percentage with which they appear.
	- This encoding can cause collisions since more than one categorical value can have same number of appearances.
- Target guided Ordered Ordinary Encoding.
	- Pretty much same as mean encoding done in FYP Movie Forecasting.
- Probability ration encoding.
- Weight of Evidence.
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-084)


## Day 83 | June 27 2020 | Saturday
Today I continued with the same course and started learning about the techniques of missing data imputation.
- Imputation is the act of replacing the missing values with statistical estimates of the missing values.
- **Remember to always use these imputers in train and test split fashion**
- Techniques for Handling the missing values.
	- CCA (complete case analysis).
		- Drop any row which has any missing value.
		- Very restrictive usage when no more than 5% of the data has the missing values.
		- Can reduce the size of the dataset drasticly.
- Mean-Medium Imputation.
	- If the variable is normally distributed the mean is a good imputer.
	- If the variable distribution is not normal then medium is a better imputer.
	- Disadvantages of this approach.
		- Distortion of the original variable distribution.
		- Distortion of the covariance with the remaining variables of the dataset.
		- Distortion of the original variance.
		- Affects the inter quartile ranges.
		- The higher percentage of the missing values, the higher the distortions.
	- Restrictive usage when no more than 5% of teh data has missing values.
- Arbitrary value Imputation.
	- For numerical values can be any number not in the of the variable.
	- For categorical values can be any label not present in the variable (Often "MISSING" is used).
	- Disadvantages of this approach.
		- Distortion in distribution, variance and covariance.
		- If the arbitrary value is from the end of the distribution, it may mask or create ourliers.
		- Affect the inter quartile ranges.
		- The higher the percentage of missing values, the higher the distortions.
- End of tail Imputation.
	- Quite similar to arbitrary value imputation.
- Frequent value Imputation.
	- Replace the missing values by mode or most frequent value of the variable.
	- Disadvantages are similar as in the previous techniques.
	- Over-representation of the frequent value in the variable.
	- The frequent value can distort the distribution and covariance of other variables with its perticular value.
- Random Sample Imputation.
	- Take random observation from all the available observations of the variable and replace it with missing value.
	- **It preserves the variance of the variable.**
	- Memory heavy since it has to store all the availabel observations.
	- Due to randomness you cannot have same dataset with repeating this process hence the results of the model trained on one version of random sample imputation dataset might differ from the other.
		- You can resolve this problem by setting the seed.
		- You should also use the same seed in the deployment.
		- You can set this seed by other available vairables (columns) interactions in the same rows (age * salary).
- Missing Indicator.
	- An additional binary variable which indicates whether the data was missing for an observation (1) or not (0).
	- It expands the feature space of the dataset.
	- Original variable still needs to be imputed.
	- Many missing indicators may endup identical or very highly correlated.
- Scikit-Learn available methods for imputation.
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-083)


## Day 82 | June 26 2020 | Friday
Today I started a new course on [Feature Engineering for Machine Learning](https://www.udemy.com/course/feature-engineering-for-machine-learning/) and completed its first couple of modules.
- Feature engineering includes dealing with missing values, categorical variable encoding, variable transformation and creating new features.
- Variables.
	- Numerical variables.
		- Discrete variables.
		- Continous variables.
	- Categorical variables.
		- Nominal Categorical variables.
			- Categorical variables for which order does not matter.
		- Ordinal Categorical variables.
			- Categorical variables where order matters.
	- Datetime variables.
	- Mixed Variables.
		- Contains both the numberic and categorical variables.
- Variable Characteristics.
	- Missing data.
		- Missing data completely at Random (MCAR). 
			- There is no relationship between the missingness of the data and any values, observed or missing.
		- Missing data at Random (MAT).	
			- There is a systematic relationship between the propensity of missing values and the observed data, but not the missing data.
		- Missing Data not at Random (MNAR).
			- There is a mechanism or a reason why missing values are introduced in the dataset.
		- To understand the mechanismby which missing data is introduced, we need to become familiar with the methods used for data collection. It also helps us defining how to best engineer the features.
	- Cardinality of the variable.
		- Possible values of a categorical values in a feature.
		- High cardinality may cause over fitting and operationalisation problems.
			- There can be an uneven split between training and testing, due to high cardinality and less examples for each label.
	- Linear Model Assumptio.
		- Independend variables are used to predict the depedend variable.
		- There is a linear relationship between dependend variables and indipendent variables.
		- The indipendent variables are not very highly correlated with each other.
		- Homoscedasiticity.
			- The error term for a given dependend variable is the same across all independent variables. 
	- Outliers.
		- A point in the data which is significantly different from the data.
		- Sometimes the outliers are important to pay attention to, for example credit card fraud detection and some times these outliers are not importatn to pay attention to, for example an error introduced by measurement.
	- Feature scalling and Feature magnitudes.
		- Higher valued variables tends to have more affect on linear models, than others variables.
- [Code base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-082)

## Day 81 | June 25 2020 | Thursday
Today I continue with the course and learned the ARIMA and its applications on time series data.
- Auto-Regressive Integrated Moving Averages.
	- Is a generalization of an autoregressive moving average model. Both of these models are fitted to time series data either to better.
	- ARIMA(1,1,1) = <sub>delta</sub>P = c + phi<sub>1</sub>* <sub>delta</sub>P<sub>t-1</sub> + theta<sub>1</sub> epslon<sub>t-1</sub> + epslon<sub>t</sub>
	- Simplistic ARIMA models.
	- High Level Arima Models.
	- Higher level of integration. 
	- Seasonality in ARIMA ==> SARIMA
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-081)


## Day 80 | June 24 2020 | Wednesday
Today I continued with the course and applied Moving averages statistical model to time series data.
- Moving Averages (MA) Model.
	- r<sub>t</sub> =c + theta<sub>t</sub>epslon<sub>t-1</sub> + epslon<sub>t</sub>
		- r<sub>t</sub> represent the value in the current period.
		- theta is a numeric coefficient.
		- epslons are the residuals of current and past lags.
	- The further back we go in time the more chances are we are overfitting.
	- MA models are not better at predicting the non-stationary data.
- Auto-Regressive-Moving Averages (ARMA).
	- A combined model with auto-regressive and moving averages.
	- r<sub>t</sub> = c + phi(r<sub>t-1</sub>) + theta<sub>1</sub>epslon<sub>t-1</sub> + epslon<sub>t</sub>
	- Higher order ARMA models.
	- ARMA for Non-Stationary data.
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-080)


## Day 79 | June 23 2020 | Tuesday
Today I continued with the course and applied Auto-Regressive statistical model to time series data.
- Picking the model.
	- Usually start with a simpler model and then expand it.
	- If expanding the model the new coefficients needs to be significantly different than zero.
- Auto-Regressive (AR) Model.
	- A linear model, where current period values are a sum of past outcomes multiplied by a numeric factor.
	- X<sub>t</sub> = C + **Phi** X<sub>t-1</sub> epslon<sub>t</sub>
		- **Phi** any numeric constant by which we multiply the lagged variable.
			- Its value is always between -1 and 1.
		- **epslon**<sub>t</sub> The difference between our prediction for period **t** and the correct value.
		- You can have many lagged values for example t-2, t-3 and so on.
	- Fitting AR Model with single lag.
	- Fittign AR Model with multiple lags.
	- Analysis and Evaluating the model using the summary.
	- Log Likely hood ratio.
	- AR Model to predict Amazon returns.
- Normalizing the values. 
	- Normalizing does not affect stationarity.
	- Does not have any affect on model selection.
		- Only the constant value is changed the rest of the coefficients are same as for the un-normalized data.
- Analysing the Residuals of the model.
	- Model results returns residuals using .resid attribute.
	- If these residuals are stationary our model is a good fit.
	- For the selected model to be better, its results residuals needs not to be significant in DickeyFuller test. If they are significant, that implies there exist an even better model to predict the data.
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-079)


## Day 78 | June 22 2020 | Monday
Today I countinued the course and started the next modules.
- White Noise.
	- It has constant mean, constant standard diviation and no-autocorrelation.
	- White noise cannot be predicted.
- Random Walk.
	- A Special type of time series, where values tend to presist over time and the differences between periods (residuals) are simply white noise.
	- Lets say P is price and **r** is residual then.
		- P<sub>t</sub> = P<sub>t - 1</sub> + **r**
	- Random walks cannot be predicted accuratly.
- Market Efficiency.
	- Measures the level of difficulty in forecasting correct future values.
- Time Series Stationarity.
	- Time series stationarity implies taking consective samples of the data with the same size, should have identical covariance, regardless of the starting point.
	- Dickey-Fuller test for testing the variable if its stationary or not.
		- Null hypothesis assumes that the variable is non-stationary.
- Seasonility.
	- Trends will appear on a cyclical basis.
		- Example would be temprature rise and fall in seasons.
		- Trend
		- Seasonality
		- Residuals.
- Auto-Correlation Plots.
- Partial Auto-Correlation Plots.
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-078)

## Day 77 | June 20 2020 | Saturday
Today I started the course on [Time series analysis](https://www.udemy.com/course/time-series-analysis-in-python/) learned the following topics.
- Time series data.
	- A sequence of information which attaches a time period to each value.
		- Time period.
		- Frequency.
	- Patterns observed in time series are expected to presist in the future.
	- Notations.
- Missing values in time series data are more complex to handle since, the values of the next periods depends upon the values of the previous periods.
- Splitting time series data for training and forecasting.
- QQ plot (Quantile Quantile Plot).
	- Y-axis represents the possible values of the variable in ordered.
	- X-axis shows the means and each tick (point on axis) is 1 standard diviation away.
	- A tool to analyse if your data is normally distributed or not.
- Setting frequencies in our time series data.
	- Setting up frequencies may introduce some missing values since there are going to be some periods which don't have any data.
- Filling missing values.
	- Front Filling.
	- Back Filling.
	- Mean Filling.
- Splittng the time series data.
- Auto correlation & Serial correlation.	
	- It is the correlation of a signal with a delayed copy of itself as a function of delay
- White Noise.
	- In time series white noise means the time series doesn't have any pattern.
[Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-077)


## Day 76 | June 19 2020 | Friday
Today I started the next modules and learned about advanced tensorflow usage and Low level tensorflow and completed the course.
- Serving tensorflow models.
- Tensorflow Lite.
	- For mobile and embedded applications.
- Low level tensorflow.
	- Constants, Variables and Gradient Tape.
- Building your own custom model.
- Indepth loss functions.
	- Mean Squared Error.
	- Binary Crossentropy.
	- Categorical Crossentropy.
- Indepth Gradient Descent.


## Day 75 | June 16 2020 | Monday
Today I continued with the previous parts of re-enforcement learning and learned the following topics.
- Re-enforcement learning.
	- Agent and Enviroment.
		- Agent takes actions according to the state of the environment and the state of the environment is changed.
	- State, action and reward.
	- Epiodes in re-enforcement learning is complete exercise of an agent to gain the reward.
- State.
	- It can be discrete (like in tic-tac-toe) or continuous (like camera etc)
- Policy.
	- Policy is what the agent uses to determine what action to take given a state.
- Markov Decision Processes.
	- It is the main assumption we make in RL.
	- It states.
		- In general, we say the probility of state **t** depends only on the state at time **t - 1**.
		- P (s<sub>t</sub> | s<sub>t-1</sub>, s<sub>t-2</sub>,   , s<sub>0</sub>) = P(s<sub>t</sub> | s<sub>t - 1</sub>)
		- The state can be a sequence of events/words/states.
- Agent tries to maximize its long term reward.
- Bellman Equation.


## Day 74 | June 15 2020 | Monday
Today I continued with the course and started the next module on Re-enforcement Learning and learnt trading using Re-enforcement learning algorithm.
- In supervised and unsupervised machine learning, you train a model and make predictions after the prediction **You** decide whether to take some action or not.
- The agent will take the action (buy, sell a stock or do-nothing) which it thinks will maximize the reward.
- Enviroment for the RL agent is the stock market itself.
- Reward is connected to whether you gianed the money or lost.
- Replay Buffer implementation.
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-074)


## Day 73 | June 14 2020 | Sunday
Today I continued the Transfer learning module of the course and moved on to the Generatrive Adverserial Networks.
- Approaches for transfer learning.
- Freezing the pretrained expensive layers during training
- Creating embeddings of input images using pre-trained models and then using simple LogisticRegression for binary classification and other classifiers for multiclass classification.
- GANs (Generative Adversarial Networks).
	- A system of 2 neural networks, each of which has their own objectives. The objective of first network is to generate images and the objective of the second network it to discriminate between real and fake images.
	- We have two loss functions in GANs, one for generator and the other for discriminator.
	- Discriminator and Generator.
		- Simple loss function binary cross entropy.
		- Freeze the layers of discriminator so they won't get updated, and only Generator will get trained.
		- Flipping the labels to fake images as 1 (assuming 1 is the label for real image).
		- Input for the discriminator is the image creted by Generator.
		- Input for Generator is just random noise from some distribution.
- Implementation of GANs on MNIST data results are [here](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-073/gans-images)
- Images generated by GANs [here](https://thispersondoesnotexist.com/)
- Game for guess which is synthetic image by GANs and which is the original image [here](http://www.whichfaceisreal.com).

- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-073)


## Day 72 | June 11 2020 | Thursday
Today I continued with the same course and started a new modules on Recommender System and Transfer learning.
- Motivation for recommendation systems.
- Sample for recommendation system is created by three items **user**, **item** and **rating**.
- General process of recommendation.
	- Embedding of the user and item under consideration.
	- Feed both embeddings to a network in parallel.
	- Predict the rating that user will give to the movie.
- Implementation of movie recommendation project.
- Transfer learning.
	- Motivation for transfer learning.
	- The basic idea behind the transfer learning is that features learned for one task might be usefull for another task.
	- Freezing the layers of the pretrained neural networks in trainsfer learning will not update the weights for these layers. 
- Some pretrained networks.
	- VGG16 & VGG19
	- ResNet50, ResNet101 and ResNet152
	- Inception
	- MobileNet 
		- Lightweight.
- Large datasets and dataset generators.
	- Loading one batch at a time for training on large datasets.
	- Data augmentation.
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-072)


## Day 71 | June 10 2020 | Wednesday
Today I started the next module of the course and worked on classifying the text using CNNs and LSTMs.
- Embeddings.
	- Dense vectorized representation of the input(image/text) where each element of the vector represent some feature of the input.
- Tensorflow Embeddings.
- Text preprocessing
	- Tensorflow Tokenizer.
	- Pad Sequences.
		- Pre-truncation and Post-truncation.
		- Its important to pad/truncate the sequence from beginning or ending since, RNNs have problems with learning long distance patterns you might wanna put the padding at the beginning. 
		- Whether to do Post-padding or Pre-padding highly depends upon the problem under consideration.
- Spam classification using LSTMs.
- Convolutional Neural Networks for text classification.
	- One dimentional Convolution.
	- Embedding layer creates vectors of each word from the sentence.
		- Each word is converted to a respective vector.
		- These vectors are stacked together to create a matrix of M x N, on this matrix convolution is performed
	- Spam classification using CNNs
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-071)


## Day 70 | June 9 2020 | Tuesday
Today I did a project on stock price prediction using the Long short-term memory neurons.
- Motivation for stock price predictions and Deep learning
- Most common mistake people do while predicting the stock prices.
- Correct way of predicting the stock returns.
- Regression is generally harder problem than classification, especially binary classification.
	- Rather than using the regression to predict the exact price of the stock we can actually use classification model to predict if the price will go up or down.
- **0%** accuracy is not a worse accuracy it means you can reverse the predictions to get 100% accuracy.
- **50%** accuracy is the worse accuracy.
- Stock price prediction is a very harder problem, we can't even predict if the stock price is going up or down then how can we predict the exact stock price.
- We need huge amount of data with huge number of features, because there are a lot of things that affect the stock prices.
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-070) 


## Day 69 | June 8 2020 | Monday
Today I continued with the Recurrent Neural module and spent most of my time doing projects.
- LSTM and Long term dependencies.
	- Using Simple RNN unit.
	- Using LSTM.
	- LSTM performs better than RNN for catpuring the long term dependencies.
		- LSTMs also have a limit for upto a certain length of dependencies.
		- Using GlobalMaxPool1D can improve the results for longer distence dependencies.
- Image Classification using RNNs.
	- Treating images as multi-dimensional time series data.
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-069)


## Day 68 | June 7 2020 | Sunday
Today I continued with Recurrent Neural Network module and starting learning the following topics and did some practical projects.
- Input/Output shapes for RNNs.
	- Number of samples, sequence length, input features length, number of hidden units and output unit.
- GRU (Gatted Recurrent Unit) and LSTM (Long short term memory).
	- Vanishing Gradient problem in RNNs.
	- GRU
		- Solution of Vanishing gradients using GRU.
		- Mathematical equation derivation.
	- LSTM
		- Solution of Vanishing gradients using LSTM.
		- Mathematical equation derivation.
- Challenging Sequence forecasting.
	- Linear Regression.
	- Simple RNN
	- GRU
	- LSTM
- [Code base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-068)


## Day 67 | June 6 2020 | Saturday
Today I started Recurrent Neural Network module studied the following topics.
- Sequence Data.
	- Introduction and motivation with time series analysis data.
	- Shape of a Sequence is represented in 3D using N x T x D.
		- N = # Samples
		- D = # features
		- T = # time steps in the sequence
	- Padding for different sequence sizes.
- Time Series Forecasting.
	- Length of time we want to predict is called horizon.
	- total_width - kernal_width + 1 = total number of windows of the kernal size.
	- Auto regressive model.
		- x<sup>^</sup><sub>t</sub> = w<sub>0</sub> + w<sub>1</sub>x<sub>t-1</sub> + w<sub>2</sub>x<sub>t-2</sub> + w<sub>3</sub>x<sub>t-3</sub>
- Recurrent Neural Network.
	- Hidden Features depend upon the input as well as the previous hidden state.
	- Unrolled RNNs example.


## Day 66 | June 5 2020 | Friday
Today I continued with the Convolutional Networks and did some projects with CNNs.
- Convolutional Neural Networks.
	- Feature learning & Classification.
		- Feature learning in the earlier to later convolutional
	- Pooling layers.
	- Use Small feature maps 3x3, 5x5 or 7x7
	- Repeat: convolution --> pooling --> convolution --> pooling -- etc.
	- Increase number of feature maps as you are going deeper in the network.
	- Larger stride for convolution for skipping the same pixels around the pixels under consideration.
	- Global max-pooling.
	- [Caculating the number of parameters in Convolutional Neural Network](https://towardsdatascience.com/understanding-and-calculating-the-number-of-parameters-in-convolution-neural-networks-cnns-fc88790d530d)
- Tensorflow Keras Functional and Sequentials APIs.
	- Fashion MNIST project implementation.
	- Cifar10 project implementation
- Data Augmentation.
	- Can be applied for certain types of data (image data) and not for others (tabular data)
	- Shift pixels, 
	- Move image up,down etc.
	- Rotation of the image.
	- Keras API ImageDataGenerator for Augmentation.
- Data Normalization.
	- Batch normalization layers after convolutional layers.
- Training Cifar10 using Data augmentation and Batch Normalization.
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-066)


## Day 65 | June 4 2020 | Thursday
Today I continued with the course and started learning about the feed forward networks and convolutional neural networks.
- Feed forward neural networks.
	- Different neurons capture different features.
	- Deeper and Wider neural networks.
	- Every neuron is a linear classifier.
	- Geometerical Interpretation.
	- Activation Functions.
		- Tanh & Sigmoid
		- Vanishing Gradient.
		- ReLU & Dead Neurons.
		- Leaky ReLU and ELU (exponential linear unit)
	- Multi-class classification.
		- Probability distribution and Softmax.
	- Representation of Images.
		- Flatten images for feed forward networks.
		- Cross-Entropy and sparse-cross-entropy loss function.
	- Classification and Regression using Feed forward network.
- Convolutional Neural Networks.
	- Convolution.
		- Valid convolution ==> No padding --> output size ==>  N - K + 1
		- Same convolution ==> Padding --> output size ==> same as before (N) 
		- Full convolution ==> higher padding --> output size ==> N + K - 1 
		- Convolution a pattern finder
		- Weight sharing via convolutional filters.
		- 3D Convolutional.
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-065)


## Day 64 | June 3 2020 | Wednesday
Today I started the course on [Tensorflow 2.0 Deep Learning and Artificial Intelligence](https://www.udemy.com/course/deep-learning-tensorflow-2/) for hands on practice and learning of the tensorflow API and some deeplearning stuff.
- Introduction & motivation & Outline.
- Google colab.
- [Code](https://github.com/lazyprogrammer/machine_learning_examples/tree/master/tf2.0)
- Introduction to Google Colab.
	- google.colab files and file uploads.
	- Mounting the gDrive with google colab.
- Machine Learning and Neurons.
	- Machine learning is nothing but just geometery problem.
	- Classification and Regression.
	- Basic Notations & Coding conventions of Tensorflow.
	- Hyper parameter and model parameters.
	- [Learning Rate scheduling](https://www.tensorflow.org/api_docs/python/tf/keras/callbacks/LearningRateScheduler)
- Classification tensorflow code along example.
- Linear Regression tensorflow code along example.
- Saving and Loading
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-064)


## Day 63 | June 2 2020 | Tuesday
Today I completed the course on [Deep learing with TensorFlow 2.0 [2020]](https://www.udemy.com/course/machine-learning-with-tensorflow-for-business-intelligence/) and did its final project with MNIST example.
- Data Preprocessing.
- Data Shuffling.
	- Buffer size.
- Model Topology
- Model training and tuning.
- Business Case Example.
	- Analysing the features and determining their importance.
	- Balancing the dataset.
	- Early stopping with Tensorflow.
		- By default will stop the training once the validation loss increases.
		- We can change this behaviour using **patience** which is an integer will allow model to continue for defined number of epochs after the loss has increased.
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-063)


## Day 62 | June 1 2020 | Monday
Today I continued the course on [Deep learing with TensorFlow 2.0 [2020]](https://www.udemy.com/course/machine-learning-with-tensorflow-for-business-intelligence/) and learnt the following topics.
- Overfitting & Underfitting.
	- Bias Variance tradeoff.
	- Trian validation and test data.
	- KFold cross-validation
	- Early stopping.
- Initialization.
	- Random initialization and activation functions.
	- Xavier/Glorot Initialization.
		- Uniform Xavier Initialization.
		- Normal Xavier Initialization.
- Optimization.
	- Batch Gradient descent.
		- Parallel batch training on multiple course.
	- Local Minimum points.
	- Momentum
	- Adaptive Learning rate.
		- AdaGrad
		- RMSprop
		- Adam
- Preprocessing.
	- Feature Scaling. 


## Day 61 | May 31 2020 | Sunday
Today I started the course on [Deep Learning with TensorFlow 2.0 [2020]](https://www.udemy.com/course/machine-learning-with-tensorflow-for-business-intelligence/) and started learning tensorflow 2.0.
- Course Introduction.
- Types of Machine Learning.
	- Supervised, Unsupervised and Re-enforcement Learning.
- A machine learning model.
	- Visual animated example of a linear model.
	- Multiple inputs and multiple outputs.
		- If there are **N** inputs and **K** outputs then there would be **NxK** weight matrix and **K** biases.
	- Cross Entropy Loss function.
	- Optimization and Learning rate.
	- A minimal example for NN model using numpy.
- Introduction to Tensorflow.
	- Support for CPU,GPU and TPU.
	- A minimal example for NN model using tensorflow.
- Introduction to Deep neural networks.
	- None linearity and hidden layers.
	- Softmax activation function.
		- A softmax activation function transforms a bunch of arbitrarily large or small numbers into a valid probability distribution.
		- Sum of all the probabilities in all the units will be 1.
	- Backpropagation.
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-061)


## Day 60 | May 30 2020 | Saturday
Today I completed the course [Projects in Machine Learning](https://www.udemy.com/course/machine-learning-for-absolute-beginners/) and did the following projects.
- Super Resolution CNNS.
	- Taking in a low resolution image and converting it to a high resolution image.
	- Matrices for image comparison.	
		- PSNR (Peak signal to noise ratio)
		- MSE (Mean Squared Error)
		- SSIM (Structural Similarity)
- KMeans clustering for image Analysis.
	- Metrics.
		- Intertia
			- Measures the spread of the clusters.
			- Increasing the number of clusters will decrease the intertial.
		- Homogeneity score
			- If all of the data points in a single cluster are the points of a single class.
			- Increasing the number of clusters will increase the homogeneity.
		- Accuracy.
- Data Compression and Visualization using PCA.
	- Elbow method.
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-060)


## Day 59 | May 29 2020 | Friday
Today I continue with the course and did the following projects.
- Object recognition using CNNs.
	- Striving for Simplicity: All Convolutional Net.


## Day 58 | May 28 2020 | Thursday
Today I continued with the course and did a couple of other projects which are as follows.
- Creadit Card Fraud Detection.
	- Anomaly detection.
	- [IsolationForest](https://towardsdatascience.com/outlier-detection-with-isolation-forest-3d190448d45e).
		- Isolation Forest is an outlier detection technique that identifies anomalies instead of normal observations.
	- [LocalOutliearFactor](https://towardsdatascience.com/local-outlier-factor-for-anomaly-detection-cc0c770d2ebe).
		- Local Outlier Factor (LOF) is a score that tells how likely a certain data point is an outlier/anomaly.
- NLTK Tagging, Chunking and Named Entity Recognition.
	- NLTK pos_tag
	- Keeping just a certain types of the entities using the pos.
- Spam Filteration.
	- Text preprocessing.
	- Multiple Model Comparison.
	- classification report
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-058)


## Day 57 | May 27 2020 | Wednesday
Today I started [Projects in Machine Learning](https://www.udemy.com/course/machine-learning-for-absolute-beginners/) course which is a hands on course for coding machine learning and deeplearning algorithms.
- Supervised Learning.
- Unsupervised Learning.
- Re-enforcement Learning example project.
	- [Open AI Docs](https://gym.openai.com/docs/#getting-started-with-gym)
	- Observation, reward, done and info when call environment.step(some_action)
	- PoleCart-v0 RL-Training.
- Game board review prediction.
	- [Dataset](https://github.com/ThaWeatherman/scrapers/tree/master/boardgamegeek)
	- Data Exploration and Visualization.
	- Data Filteration.
	- LinearRegression and RandomForests
- [Code Base](https://github.com/mohsin-ashraf/personal-msds-1/tree/master/codebase/day-057)


## Day 56 | May 26 2020 | Tuesday
Today I completed the course on nlp.
- Sense (or word sense).
	- Discrete representation of an aspect of a word's meaning.
		- Homographs (bank/bank, bat/bat)
		- Homophones (write/right, Piece/peace)
		- These phenomenon causes a number of problems in NLP tasks
	- [WordNet](http://wordnetweb.princeton.edu/perl/webwn) and other Online Thesauri
		- Word similarity and Thesaurus Methods.
			- Path based similarity in the Thesaurus.
		- Distributional Similarity.
			- If **A** and **B** have almost identical environments we say that they are synonyms.
			- Column vector similarity of sentences (TF count)
			- Row vector similarity of words (TF along the row)
			- Cosine Similarity
- Question Answering.
	- Answer types and query formulations.
	- Ranking of condidate answers.
	- Using Knowledge in QA.
		- Databases of Facts, Relations and others.
		- Validity of answers by their attributes (if a person is died in 1990s he won't be alive in 2000s etc.)
- Introduction to Summarization.
	- Extractive Summarization.
		- Create summary from the phrases or sentences in the source document.
	- Abstractive Summarization.
		- Express the ideas in the source documents using different words.
	- Evaluating Summaries ROUGE (Recall Oriented Understudy for Gisting Evaluation)
 

## Day 55 | May 25 2020 | Monday
Today I continued with the nlp course and started learning about the POS tagging.
- Intro to part of speech and POS tagging.
	- Words often have more than one POS.
	- Sequence Models for POS Tagging.
		- Bi-directional Sequence models.
- Statistical Natural Language Parsing.
	- Constituency Parsing.
	- The Exponential problem in parsing.
- Context Free Grammar (CFG) and Probablistic Context Free Grammar (PCFG).
- Chumsky Normal Form.


## Day 54 | May 24 2020 | Sunday
Today I continued with the nlp course and started learning about Information Extraction, Named Entity Recognition and Relation Extraction.
- Named Entity Recognition (NER).
	- Finding and classifying the attributes and their values in the text.
		- For example, Person, Location, Organization etc.
		- Usage of NER.
	- Evaluation of Named Entity Recognition.
		- Precision, Recall and F1 for statistical measures.
		- The boundaries of collected entities are correct or not.
	- Sequence Models for NER.
		- IO Encoding of text data.
		- IOB Encoding of the text data. 
	- Maximum Entropy Sequence Models.
- Relation Extraction.
	- Extracting facts about the entities from the text. (e.g Stanford was founded in 1891 or maybe extracting family relationships husban & wife).
		- Using Patterns to extract relationships.
		- Using grammatical knowledge for relation extraction.
		- Trigger words for relations (e.g parent, son and brother etc for family)
	- Supervised Learning for Relation Extraction.
		- First classify if the entities are related or not.
		- If yes, then classify the relationship between the entites.
	- Semi Supervised and Unsupervised Relation Extraction.


## Day 53 | May 23 2020 | Sutarday
Today I started learning about the Discriminative Models.
- [Generative vs Discriminative models](https://stackoverflow.com/questions/879432/what-is-the-difference-between-a-generative-and-a-discriminative-algorithm).
-  Making features from text for Discriminative NLP models.
	- Quality of the features are much more important than the model you choose.
- Feature based Linear Classifiers.
	- Learn linear function from the features to classes.
- Maximizing the Likelihood.


## Day 52 | May 22 2020 | Friday
Today I continue witht the course and started learning about sentiment analysis.
- Extracting sentiments of people about the product or service.
	- Sentiments about the attributes of the products.
	- Holder of attitude, Target of attitude, Type of attitude and Text containing the attitude.
- Base line algorithm for sentiment classifiction.
	- Preprocessing.
		- Normalization of the text.
	- Feature extraction.
		- Negation.
	- Applying the classifier.
	- Occurrence of word tells a lot more than the frequency of its occurrence.
		- For sentiment analysis we sometime clip the frequency of the word.
- Sentiment Lexicons
	- Polarity and Subjectivity.
- Learning Lexicons
	- Adjectives conjoined by "and" have same polarity.
	- Adjectives conjoined by "but" do not have same polarity.
	- Co-occurrence.
	- Sinonyms of the words have the same polarity. 
- Challenges in sentiment classification.
	- Seemingly positive review but actually negative.


## Day 51 | May 21 2020 | Thursday
Today I continued with the course of NLP and learned the following topics.
- Text classificaion.
- Naive Bayes Classifier one of the most important text classification algorithm.
	- Formalizing the Naive Bayse Classifier.
		- Assume the feature probabilities are independent given the class c.
	- Naive Bayes Learning.
	- Naive Bayes relationship to the Language Model.
	- Multinomial Naive Bayes: A worked Example.
- Precision Recall and F1 score.
- Text classification evaluation.
	- Macro-averaging.
	- Micro-averaging.
- Practical Issues in Text Classification.


## Day 50 | May 20 2020 | Wednesday
Today I continued with the course of NLP and learned the following topics.
- Backoff and Interpolation.
	- Interpolation works better than Backoff.
	- Simple Interpolation.
	- Context conditional Interpolation.
- Pruning to compute the probabilities for large scale n-grams (e.g Google N-gram corpus)
	- Caching models.
		- Recently used words are more likely to appear.
			- works poorly on speech data.
- Good turing Smoothing.
	- Use the count of things we have seen once to help estimate the count of things we have never seen.
	- N<sub>c</sub> = Frequency of frequency c (How many things occurs with frequency **c**)
	- P<sup>* </sup><sub>GT</sub> (things with zero frequency) = N<sub>1</sub>/N  c<sup>* </sup> = (c+1)N<sub>c+1</sub>/N<sub>c</sub>
- Kneser Ney smoothing.
- Spelling correction.
	- None words Errors
		- graffe ---> giraffe where graffe is not a word of english.
		- Use large dictionary to detect these kind of errors, any word not in the dictionary is an error, the larger the dictionary the better.
	- Real-word Errors.
		- Typographical Errors.
			- three ---> there.
		- Cognitive Errors.
			- piece ---> peace
	- Spelling correction and the noisy channel.
		- Language models.
	- State of the art systems.
		- Auto-correction (fully confident)
		- List of corrections.
	- Finally multiple approaches can be combined to deal with the spelling correction including language modeling, pronunciations, Homology on the key board and many others.


## Day 49 | May 19 2020 | Tuesday
Today I continued with the course and learned the following topics.
- Probabilistic Language Modeling.
	- Markov Assumption.
	- P(the | its water is so transparent that) ~ P(the | that)
	- P(the | its water is so transparent that) ~ P(the | transparent that)
	- N-grams and long distance dependencies.
- Estimating the N-gram probabilities.
	- bi-gram probability ==> P(w<sub>i</sub> | w<sub>i - 1</sub>) = count(w<sub>i-1</sub>,w<sub>i</sub>)/count(w<sub>i-1</sub>)
	- Converting it to log space to avoid underflow of tiny tiny probabilities when multiplying them togather.
		- p<sub>1</sub> X p<sub>2</sub> X p<sub>3</sub> =   log(p<sub>1</sub>) + log(p<sub>2</sub>) + log(p<sub>3</sub>) 
- Evaluation and Perplexity.
	- Extrinsic Evaluation.
- Generalization and Zeros.
	- N-grams only works well for word prediction if the test corpus looks like the training corpus.
	- Add-one smoothing or Laplace smoothing.


## Day 48 | May 18 2020 | Monday
Today I started the [course](https://www.youtube.com/playlist?list=PLQiyVNMpDLKnZYBTUOlSI9mi9wAErFtFm) on NLP by Dan Jurafsky, Christopher Manning on YouTube and learned the following topics.
- Motivation for NLP and course outline.
- Challenges in NLP domains.
- Basic Information extraction using Regex.
	- [regexpal.com](https://www.regexpal.com/)
	- In pattern matching fixing False Positives and False Negatives.
	- Regular Expressions in practical NLP.
- Word tokenization.
	- Unix tools for text processing.
	- **tr** for command line text processing.
	- Complications and tokenizatoin.
	- Rules for different languages are different.
	- Max-match segmentation.
		- Does't generally work for English.
- Word Normalization and Stemming.
	- Lemmatization. 
	- Porter Stemmer.
- Sentence Segmentation.
	- Split sentences is a problem due to these words P.hD, 2.43 Dr. U.S.A etc.
- Minimum Edit Distance.
	- Minimum number of editing operations needed to transform one string to another.
		- Insertion
		- Deletion
		- Substitution
	- In Levenshtein distance the substitution cost is 2 (one for deletetion and one for updation).
	- Solving minimum edit distance using Dynamic Programming.
	- Backtrace for computing alignment.
	- Weighted edit distance computation.
	- Minimum Edit Distance in Computational Biology.


## Day 47 | May 17 2020 | Sunday
Today I completed the deep learning specialization assignments and quizzes and completed the deep learning specialization.
- Speech recognition.
	- Given an audio clip **x** the task is to find a transcript **y**.
- Trigger word detection.
- Assignments and quizzes completion.


## Day 46 | May 16 2020 | Saturday
Today I continued with the final module of the final course of the deep learning specialization and leaned the following topics.
- Beam Search for language models.
	-  Will pick N most likely words for a language translation given a word **x** of another language i.e P (y|x) where y = a,b,c and a,b,c are the most likely words that the beam search selected for language L1 given a word x from languge L2 (here N = 3).
- Refinements to Beam search.
	- Length normalization can help us get better results.
		- 1/T<sub>y</sub><sup>alpha</sup> SUM <sub>t = 1</sub><sup>	Ty </sup>log P(y<sup>t</sup> | x, y<sup>< 1 ></sup>, y<sup>< 2 ></sup> ,   , y<sup>< t - 1 ></sup>)
	- The larger the width of the Beam Search (selecting N to be greater) the more possibilities you are considering and hence the more better translations you can get. But the down side is that it requires computational power.
- Error Analysis on Beam search.
- Bleu Score.
	- Measures how good the translation created by machine is, or how close the translation created by machine is to the translation done by human.
- Attention Model Intuition.
- Implementation details of attention models.


## Day 45 | May 15 2020 | Friday
Today I completed the quizzes and assignments of second module and started the third and last module of this course and also of this series and learned the following topics.
- Sequence to Sequence models.
	- Image captioning.
		- Use a pretrained network let say (AlexNet) and use the second last layer of the network as an input layer to the RNN model.
- Picking the most likely sentence.
	- Machine translation as building a conditional language model.
		- P (y<sup>< 1 ></sup>, y<sup>< 2 ></sup>,  , y<sup>< t ></sup> | x<sup>< 1 ></sup>, x<sup>< 2 ></sup>,  , x<sup>< t ></sup> )


## Day 44 | May 14 2020 | Thursday
Today I completed the second module of the deep learning specialization part five Sequence models and learned the following topics.
- Negative Sampling.
	- Pair of positive and negative samples.
	- Binary classifiers of vocab size (a layer of binary classifiers with vocab_size units), with **K** classifiers learning at a time.
- Glove word vectors.
	- X<sub>i,j</sub> = Number of times the word **i** (target) appears in the context of word **j** (context).
	- minimize Sum<sup>m</sup><sub>i</sub>Sum<sup>m</sup><sub>j</sub> f(X<sub>i,j</sub>)(theta<sub>i</sub><sup>T</sup>e<sub>j</sub> + b<sub>i</sub>+b<sub>j</sub><sup>'</sup>  - log(X<sub>i,j</sub>))<sup>2</sup>.
- Sentiment Classification using embeddings.
- Debiasing the word embeddings.
	- Identify bias direction.
	- Neutralize: For every word that is not definitional, project to get rid of bias.
		- Maybe first train a classifier to get the definitional words.
	- Equalize pairs.


## Day 43 | May 13 2020 | Wednesday
Today I started the second module of deep learning specialization part five Sequence models and learned the following topics.
- Featurized representation of words: Words Embeddings.
- Learning a feature vector against words, so that, these features can be used to know the semantic of a word.
	- Similary objects will have very similar representation e.g *apple ~= orange*.
- Visualization of word embeddings by reducing its dimensions (plotting it will clearly show the relationship between similar objects).
- Using pre-trained words embeddings (on let say 1B-100B words) for transfer learning.
- Continue finetuning the word embeddings with new data (if you have large dataset optional).
- Word Embeddings are quite usefull for the tasks like summarization and Named entity recognition.
- Word Embeddings are less usefull for the tasks like Language modeling and Machine translation.
- Properties of word embeddings.
	- Learn anology reasoning e.g man --> women as king --> *Queen*.
	- Cosine Similarity ==> Sim(U,V) = (U<sup>T</sup>V)/(||U|| * ||V||).
- Embedding matrix.
	- Selecting a perticular word column from embedding matrix using one hot vector of that perticular word.
- Learning word embeddings.
	- Taking word embeddings of a sentence and feeding it to the networks (to maybe predict the next word).
		- These embeddings can sometimes when stacked together can get thousands of dimensional vector, hence to reduce the dimensionality only a window of few previous words is used (let say 5-10 previous words).
		- You can also take constant number of words from before and after the target word.
- Skip gram model.
	- Randomly taking an input word and then learning a maping to some target word.
	- Iterating the above process for a few times with the same input word.


## Day 42 | May 12 2020 | Tuesday
Today I continued with the deep learning specialization part five Sequence Models completed the first module and its quizzes and assignments.
- Gated Recurrent Unit.
	- Helps in capturing the long term dependencies and overcomes the problem of vanishing gradient.
	- Memory unit.
- Long Short Term Memory (LSTM).	
- Bi-directional RNN (BRNN).
	- Has both forward and backward components.
	- y<sup>'</sup> = g (W<sub>y</sub>[a<sup> --> < t ></sup>,a<sup> <-- < t ></sup>] + b<sub>y</sub>)
- Deep RNNs.


## Day 41 | May 11 2020 | Monday
Today I started deep learning specialization part five Sequence models and started its first module.
- Motivation for sequence models.
- Notations for sequence models.
- Why not regular neural networks for sequence models.
	- Inputs and Outputs can be of different lengths in different examples.
	- Doesn't share features leaned across different positions of the text.
- At each time stamp the Recurrent neural network passes its activations to the next time stamp.
- Forward propogation is Recurrent Neural networks.
	- a<sup>< t ></sup> = g(W<sub>aa</sub>a<sup>< t - 1></sup> + W<sub>ax</sub>X<sup> < t ></sup> + b<sub>a</sub>)
	- y<sup>'< t ></sup> = g (W<sub>ya</sub>a<sup>< t ></sup> + b<sub>y</sub>)
- Backpropogation through time.
	- Logistic Loss function
- Different types of RNNs.
	- Many to many architecture (Sequence to Sequence)
	- Many to one architecture (Sequence to one number)
	- One to One architecture
	- One to many architecture
	- Encoder and Decoder
- Language modeling and sequence generation.
	- Large corpus of the language.
	- Probablistic estimations of the words appearing given previous words.
	- P(y<sup>< T ></sup>) = P (y<sup>< T ></sup> | y<sup>< 1 ></sup>,y<sup>< 2 ></sup>, ,y<sup>< T - 1 ></sup>)
- Sampling novel sequences.
- Vanishing/Exploding Gradients with RNNs.
	- Long term dependencies in languages.
	- Gradient clipping for gradient exploding.


## Day 40 | May 10 2020 | Sunday
Today I completed the certification of deep learning specialization part four by completing all the required assignments and quizzes. The relevant certificate can be found [here](https://www.coursera.org/account/accomplishments/certificate/ZZUFQ8NFYQTY)


## Day 39 | May 9 2020 | Saturday
Today I started working on the programming exercises and quizzes of the deep learning specialization part 4 and completed exercises and quizes of first two modules.


## Day 38 | May 8 2020 | Friday
Today I completed the certification of deep learning specialization part three by completing all the required assignments and quizzes. The relevant certificate can be found [here](https://www.coursera.org/account/accomplishments/certificate/KBJ9H37EG6RL)


## Day 37 | May 7 2020 | Thursday
Today I completed the certification of deep learning specialization part two by completing all the required assignments and quizzes. The relevant certificate can be found [here](https://www.coursera.org/account/accomplishments/certificate/JKHPHS87S7M4)


## Day 36 | May 6 2020 | Wednesday
Today I completed the certification of deep learning specialization part one by completing all the required assignments and quizzes. The relevant certificate can be found [here](https://www.coursera.org/account/accomplishments/certificate/WR79VC6AWN63)


## Day 35 | May 5 2020 | Tuesday
Today I started working on the programming exercises and quizes of the deep learning specialization part 1 and completed exercises and quizes of first two modules.


## Day 34 | May 4 2020 | Monday
Today I revisited the neural style transfer from deep learning specialization part 4 to clear up a couple of things which were left unclear last time.


## Day 33 | May 3 2020 | Sunday
Finally I completed the deep learning specialization part 4 for convoutional neural networks.
- One-shot learning problem.
	- Recognize the person given one single image.
	- Neural network learns the similarity function.
		- f(image_1,image_2) = degree of difference between images.
		- f(image_1,image_2) > threshold then the persons are same otherwise different.
- Siamese network.
	- Outputs the encoding of the input images.
	- If the images are of the same person the difference between the encodings must be small.
	- Apply the backpropogation to learn the function.
- Triplet loss function.
	- Looking at 3 images (examples).
		- One image is sample, the other is positive example (image of the same person) and third one is a negative example (image of another person.)
	- || f(A) - f(P) ||<sup>2</sup> + alpha <= ||f(A) - f(N) ||<sup>2</sup>
	- Loss function.
		- L(A,P,N) = max(||f(A)-f(P)||<sup>2</sup> - ||f(A) - f(N)||<sup>2</sup> + alpha , 0)
	- Data set need pairing.
		- Pair(A,P) similar and Pair(A,N) different.
- Face verification.
	- Use siamese networks for face verification with sigmoid unit in the last layer.
	- Chi-squared similarity.
- Neural style transfer.
	- Generate a new image (G) from content image (C) and style image (S).
	- Features learnt by the convolutional layers of the networks.
	- Cost function for NST (neural style transfer).
		- J(G) = alpha * J(C,G) + beta * J(S,G).
		- Apply gradient descent on this cost function.
	- Content cost function.
		- Say you use hidden layer **l** to compute content cost.
			- The earlier the layer **l** in the network more it will force to get the similar image to the content image and vice versa.
		- Use pre-trained network (may be VGG).
		- Let a<sup>[l][C]</sup> and a<sup>[l][G]</sup> be the activations of layer **l** for both images.
		- If a<sup>[l][C]</sup> and a<sup>[l][G]</sup> are similar, both images have similar content.
		- Take the element wise difference between the activations of the both images.
		- Apply gradient descent to insentivise your algorithm to make the image as closer to the content as you want.
	- Style cost function.
		- Say you are using layer **l's** activation to measure "style".
			- N<sup>h</sup>, N<sup>w</sup> and N<sup>c</sup> be height , widths and channels.
		- How correlated the activations across different channels are.
		- Style matrix computatoin.
- Convolution in 1D, 2D and 3D.


## Day 32 | May 2 2020 | Saturday
Today I continued the deep learning specialization part 4 for convolutional neural networks.
- While object detection your model need to detect one object only once.
- Non-max Suppression example.
	- Use IOU (intersection over union) to check the neighboring windows if they are overlapping with the same window which has highest probability of detection or not, if that's the case it will keep the highest probability region and discard others.
- Anchor boxes.
	- Detecting multiple objects in the image.
	- Using multiple anchor boxes to detect objects.
- YOLO (you only look once) algorithm.
	- Sliding windows for the image.
	- Apply Anchor boxing.
	- Apply Apply Non-max Suppression.
- Region Proposals.
	- Propose a regions where there might be an object to detect.
	- Run classification only on that region.
	- Its quite slow.
- Face verification vs. face recognition.
	- Verification.
		- Input Image, name/ID.
		- Output whether the input image is that of the claimed person.
	- Recognition.
		- Has a dataset of K persons.
		- Get an input image.
		- Output ID if the image is any of the K persons (or "Not recognized").


## Day 31 | May 1 2020 | Friday
Today I continued with deep learning specializatino part 4 for convolutional neural networks, and learnt about the object detection.
- Object localization.
	- Ouputing not just the object class, object presence but also its x,y and height and width.
	- The label **y** for the images would also be containing this information (like if there is an object, object class and the boundary parameters).
	- Loss function.
- Landmark detection.
	- Giving labels where you also specify the landmark points (x,y).
		- You can have as many points for land mark as you want.
- Object detectoin.
	- Sliding windows detection.
	- Train network on tightly cropped images of the object.
	- Take a window and slide it over any input image (not tightly cropped) and pass those window cropped part of the image to the network to predict whether the object is present or not.
	- Multiple slidings with different sizes of the window.
	- Computational cost for this operation is high.
- Convolutional implementation of sliding windows.
- Intersection over union (IoU).
	- Area of the overlaped boxes divided by the total area coverd by the boxes.


## Day 30 | April 30 2020 | Thursday
Today I continued with deep learning specialization part 4 for convolutional neural networks,explored the architectures of the CNNs and learnt following topics.
- Neural networks architectures.
	- LeNet - 5 architecture.
	- AlexNet architecture.
	- VGG -16 architecture.
- Very very deep neural networks are difficult to train due to the fact of exploding/vanishing of the gradient.
- Residual Networks (ResNet).
	- Skip connections.
- Network in Network.
	- One by One convolution.
- Inception model.
	- Using multiple filters with different sizes on a single convolutional layer along with pooling filters keeping the output dimension same for all the filters.
	- Let the network decide which filter will be best to use.
	- Requires very high computational cost.
	- Bunch of inception modules are combined to create a single Inception model.
- Open source implementation.
- [Transfer learning.](https://towardsdatascience.com/a-comprehensive-hands-on-guide-to-transfer-learning-with-real-world-applications-in-deep-learning-212bf3b2f27a)
- Data Augmentation.
	- Artificially creating the data.
	- Flipping, RGB variation and cropping.
- State of computer vision. 


## Day 29 | April 29 2020 | Wednesday
Today I started the deep learning specialization part 4 for convolutional neural networks, and learnt the following things.
- Motvaion for computer vision.
- Convolution operation & Edge detection.
- If you convolve an image of N<sup>2</sup> with a filter of f<sup>2</sup> the output image size would be (N-f+1)<sup>2</sup>. It shrinks the output image.
- Padding is used to overcome shrinking of the image to avoid image to become too small if your network is too deep. 
	- p = (f-1)/2 where f is usually odd.
- Strided convolution.
	- Image size after strided convolution: floor((n+2p-f)/s + 1) where s = stride size.
- Convolution on volumes (3D (RGB) images).
	- Filter for this convolutional will also be 3D.
	- Output will be a R<sup>2</sup> image.
	- We can have as many filters as we want or need.
- One layer of convolutional neural network.
- Simple Convolutional network example from feature learning to predictions.
	- Convolutional Layer (Feature learning)
	- Flatten (fully connected) layers.
	- Output layer.
- Pooling layer.
	- Max pooling, Min Pooling and Average pooling.
	- Has hyperparameters to tune, but no learnable parameters (through gradient descent).
- Example of convolutional neural network LeNet.
- Why using Convolutional neural networks.
	- Parameter sharing.
		- A feature detector that's useful in one part of the image is probably useful in another part of the image.
	- Sparsity of connections.
		- In each layer, each output value depends only on a small number of inputs.


## Day 28 | April 28 2020 | Tuesday
Today I completed the deep learning specialization part 3.
- Addressing the data missmatch.
	- Try to understand the differences between the training and the dev, test set. 
	- Artificial data synthesis.
	- Problem of sythesis only the subset of the data. (for example creating only a few types of cars and not all type of car images)
- Transfer learning.
	- pre training and fine tunning.
	- Transfer learning from A ---> B.
		- Apply transfer learning when problem A and B have the same type of input X.
		- You have lot more data for problem A than problem B.
		- Low level features learnt from problem A can be very helpful for problem B.
- Multitask learning.
	- When you have same problem. (e.g reconizing sign boards, cars and roads)
- End to End Deep learning.
	- Avoiding pipelines for different steps and performing input to output map in a single neural network.
		- You need to have a lot of data.
- Whether to use end to end deep learning.
	- Need a huge amount of data.


## Day 27 | April 27 2020 | Monday
Today I continued with the deep learning specialization part 3.
- Error Analysis.
	- Manually examining the mistakes made by the model.
	- Checking the labels of the miss-classified samples (small sample) manually to confirm if the labels are correct. 
	- Preparing spread sheet for better analysis.
- Cleaning up the incorrectly labelled data.
	- Small number of hours of manually examination can help you figure out the real problem and can solve the problem much quickly than randomly changing paramters and algorithms.
- Build your first machine learning system quickly and then iterate over it again and again to improve.
- Training and testing on different distributions.	
	- Randomly shuffle the distributions of the sets. 
- Bias and Variance with miss-matched data.
	- Train, train-dev set, dev set and test set.
	- Data miss-match 
	- Variance & bias problem.


## Day 26 | April 26 2020 | Sunday
Today I started the deep learning specialization part 3 for structuring the machine learning projects. 
- Orthogonalization in machine learning model improvement.
	- Using specific set of hyperparamters to tune the model performance.
- Single value model evalueation, F1 score and Accuracy.
	- Precision and Recall.
	- False Positives and False Negatives.
	- True Positives and True Negatives.
- Satisficing and Optimizing metrics.
	- if you have N metrices optimize one as much as you can by keeping N-1 as satisficing as possible.
- Train, Validation and Test.
	- Keep the distribution same.
	- Random shuffle of data.
	- Size of the train, validation and test sets.
- Evaluation of metrics also depends upon the user exceptance and company vision and needs.
- You can even customize you error function for a perticular class to be predicted or not predicted by either multiplying with a constant.
- Human level performance and even better.
	- Avoidable bias.
	- Understanding human level error/performance.
		- Team of expert radiologists classifying images.
	- Variance also needs to be reduced while achieving or surpassing human level performance.
- Improving model performance.


## Day 25 | April 25 2020 | Saturday
Today I completed the deep learning specialization part 2.
- Grid Search.
- Random selection of parameters (Sampling randomly).
- Exploitation of the parameter space where the results are better.
- Using an appropriate scale for random selection.
	- Example for tuning alpha
		1. r = -x * np.random.rand()  where x < 0
		2. alpha = 10<sup>r</sup>
	- Example for tuning mumentom.
		1. r = [-x,-y] where -x < -y < 0
		2. beta = 1 - 10<sup>r</sup>
- Expert knowledge via reading research papers and experimentations.
- Babysitting approach for tunning hyperparameters.
	- Keep monitering the learning curve (or loss curve) and change parameters accordingly.
- Training multiple models in parallel with different hyperparameter optimization.
- Batch normalization.
	- Makes hyperparameter search problem much easier.
	- Essentially it makes the neural networks much more robust against the choice of hyperparamters.
	- Can work very well even in a very big range of paramters.
	- Easily train deep neural networks.
	- Batch normalization normalizes the data comming from the hidden layers and going into the hidden layers throughout the network.
		- Normalizing the *Z<sup>[l]</sup>* where *Z<sup>[l]</sup> = W<sup>[l]</sup>y<sup>'[l-1]</sup>*
		- For normalization you can choose any distribution that fits your problem.
	- Applied with mini-batches.
	- Understanding of why does batch normalization works.
	- Make weights in the later layers (say 10<sup>10th</sup>) more robust to changes than earlier layers.
	- If you learn a mapping of **X --> y** if distribution of **X** changes then the model might need to be re-trained.
	- Batch Normalization actually reduces the problem of distribution among the layers.
	- Batch Normalization at Test Time.
		- Use estimated exponentially weighted average (across mini-batches)
- Softmax Regression.
	- Choose the close with maximum probability for more than 2 class classification problem.
	- Training with softmax classifier.
- Local optima problems in high dimentional space.
- Introduction to tensorflow deeplearning framework.


## Day 24 | April 24 2020 | Friday
Today I started with Gradient checking and moved on to learn new topics on hyperparameter optimization.
- Gradient checking.
	- Checking the value of original gradient against gradient generated after adding nudges to the weights. 
	- Gradient checking does not work with Dropout.
- Optimization Algorithms.
	- Mini-batch Gradient Descent.
	- Mini-batch Gradient Descent implementation.
	- Batch vs Mini-batch Gradient Descent (curve for loss drop).
		- For stochastic Gradient Descent keep the mini-batch 1.
	- [Important Optimization of Gradient Descent](https://ruder.io/optimizing-gradient-descent/)
	- Exponentially weighted averages.
		- V<sub>t</sub> = *B*V<sub>t-1</sub> + (1-*B*)x<sub>t</sub> :. *B = 0.9*
	- Exponentially weighted averages implementation. 
	- Gradient Descent with momentum.
		- Almost always faster than simple Gradient Descent.
	- RMSprop.
		- Controlls the learning rate in different directions according to the need.
	- Adim (Adaptive moment estimation) Optimization Algorithm.
		- Works fine for a large range of deep learning algorithms.
		- Combine both momentum and RMSprops.
	- Learning Rate Decay.
		- implementation of Learning Rate Decay.
		- *alpha = (1/(1+decay_rate * epoch_number)) * alpha*
		- *a = small_constant<sup>epoch_number</sup>* small_constant < 1.


## Day 23 | April 23 2020 | Thursday
Today I started learning more about hyperparamter optimization for neural networks.
- Regularization.
	- L1 & L2 regularization.
- Regularization penalizes the weights to reduces the overfitting.
- Dropout Regularization.
	- Randomly shutdown some of the units in the network.
	- For larger layers use high value for dropout (since larger layers have larger weight matrix).
- Dropout implementation.
- Why does Dropout Work.
	- Can't rely on any one feature, so have to spread out weights.
- Other regularizations.
	- Data augmentation.
	- Early Stopping.
- Input Normalization for neural networks.
	- Bring all features to a common scale.
- Vanishing/Exploding Gradient.
	- The slope of the functions either get exponentially small or exponentially large.
- Solution to Vanishing/Exploding Gradient.
	- Random initialization.
	- The larger the number of neurons the smaller the values of connected weights should be.
	- Example random initialization: W<sup>[l]</sup> = np.random.randn(shape) * np.sqrt(1/n<sup>[l-1]</sup>)
- Numerical Approximations of Gradients.


## Day 22 | April 22 2020 | Wednesday
Today I completed the deep learning specialization part 1 and went on for the second part. The progress for today is given below.
- Building blocks of a neural network.
- Forward and Backward propogation.
- parameters and hyperparameters.
	- hyperparameters.
		- Learning rate.
		- Activation Function.
		- Number of layers.
		- Number of layer to choose.
		- Loss function.
	- parameters.
		- weights & biasis.
- Finding suitable hyperparameters is an iterative process.
- Train, Validation and Test set split.
- Generally train = 60%, validation = 20% and test = 20%.
	- Distribution of the data across these folds matters alot.
- When using Big Data (for example 1,000,000 rows).
	- You can take the validation/test set even smaller than 20% (for example 10,000).
	- The idea for validation/test set is to find out if the model is performing better or not.
	- Sometimes this split can be train = 99.5, validation = 0.25 and test = 0.25, when you have 10s of 100s of millions of samples.
	- Destribution of the data matters alot in these splits.
- Bias and Variance trade off.
- Basic machine learning recipe. 
	- Try to figure out problems in your model.
	- Fix them one by one.
	- Iterative process. 


## Day 21 | April 21 2020 | Tuesday
Today I started derivatives of activation functions, backpropogation for neural networks.
- Derivatives of the activation functions.
- Gradient descent and Backpropogation implementation details.
- Random initialization.
- Deep neural network.
- Forward pass for deep neural networks.
- Dimensions of matrices for deep neural networks.
- Motivation why deep representation of neural networks.
	- With shallow neural networks we would required to have exponential units.


## Day 20 | April 20 2020 | Monday
Today I kept going with the deep learning specialization part one and learned following things.
- Neural network overview.
- 2 layers neural network.
- implementation instructions for neural networks.
- Explaination of vectorized implementation.
- Activation Functions.
	- Sigmoid
	- ReLU
	- tanh
	- leaky-ReLU
	- softmax


## Day 19 | April 19 2020 | Sunday
Today I started the deep learning specialization, and started the first course.
- Course overview and motivation for deeplearning.
- Simple neural network example.
- Supervised learning and types of neural networks.
- Learning curve of deep neural network with respect to the amount of data (and comparision with other ML algorithms).
- Feature vectors of data (images). 
- Sigmoid function and bias.
- Logistic regression cost function.
	- *Cost(y, y<sup>'</sup> ) = - ( (y)log(y<sup>'</sup>) + (1-y)(log(1-y<sup>'</sup>)))*
	- Interestingly one of the two term gets 0 depending upon the *y* values (0,1).
- Gradient Descent.
- Intuition of derivatives.
	- Slope of the function with respect to some given variable *x*.
- Computation Graphs.
	- Computation Graph example.
- Logistic Regression Gradient Descent.
- Vectorization and explicite for loops.
- Logistic Regression and Gradient Descent vectorization.	


## Day 18 | April 18 2020 | Saturday
Today I started learning the Eigen Decomposition, Singular Value Decomposition.
- Eigen Decomposition.
	- Defined for only squared matrices.
	- Eigen Values & Eigen vectors.
	- For *NxN* matrix there are *N* eigen values and *N* eigen vectors.
	- If **Av =** *y***v** given that **A** is a matrix, **v** is a vector and **y** is a scaler. Then **v** is an Eigen vector for matrix **A** and *y* is the eigen value.
	- Eigen Decomposition process.
		- Take the diagonal elements and subtract *Y* assuming *Y* to be an eigen value.
		- Take determinent of the matrix.
		- Find all the possible values of *Y* (which are going to be generally *N* given that matrix is *NxN*).
		- In the initial step replace all the appearances of *Y* with one eigen value at a time and find a vector which is in the Null space of the matrix ignoring the trivial case.
		- This vector is the eigen vector.
	- Diagonalization.
- Singular Value Decomposition.
	- Conceptually similar to Eigen decomposition but it can work with rectangular matrices as well, by multiplying a matrix with its transpose. 
	


## Day 17 | April 17 2020 | Friday
Today I started learning about the matrix inverses, orthogonalities & Projections and Matrix least square for model fitting.
- Matrix Inverse equation.
	1. **Ax = b**
	2. **A<sup>-1</sup>Ax = A<sup>-1</sup>b**
	3. **Ix = A<sup>-1</sup>b**
	4. **x = A<sup>-1</sup>b**
	- Matrix inverse is side-dependent.
- Matrix inverse using row reduction echelon form.
	- Agumentation of Identity matrix with the original matrix **(A | I)**
	- Converting the original matrix to identity matrix using linear operation which will broadcast along to Identity matrix as well.
	- At the end if you get an identity matrix for the original matrix (on left) you have the inverse matrix of the original matrix (on the right size).
	- If you get zeros in any row of the original matrix during this process then the solution does not exist.
	- **(A|I) ==> (I|A<sup>-1</sup>)**
- Projections and orthogonalization.
	- Projection of point *b* on a vector **a** with some scaler *B* in R<sup>2</sup> is given as.
		1. **a<sup>T</sup>** (b-**a**B) = 0
		2. **a<sup>T</sup>** b - **a<sup>T</sup>a** B = 0
		3. **a<sup>T</sup>a** B = **a<sup>T</sup>** b
		4. B = **a<sup>T</sup>** b / **(a<sup>T</sup>a)**
	- Projection of point *b* on a matrix **A** with some vector **x** in R<sup>N</sup> is given as.
		1. **A<sup>T</sup>**(b - **Ax**) = **O**
		2. **A<sup>T</sup>** b - **A<sup>T</sup>Ax** = **O**
		3. **A<sup>T</sup>Ax** = **A<sup>T</sup>** b
		4. **(A<sup>T</sup>A)<sup>-1</sup> (A<sup>T</sup>A)x = (A<sup>T</sup>A)<sup>-1</sup>A<sup>T</sup>** b
		5. **x = (A<sup>T</sup>A)<sup>-1</sup>A<sup>T</sup>** b
		6. **x = A<sup>-1</sup>A<sup>-T</sup>A<sup>T</sup>** b
		7. **x = A<sup>-1</sup>** b
	- Orthogonal & parallel vector components.
	- Orthogonal Matrices.
	- Gram-Schimdt and QR decomposition.
- Least squares for model fittings.
	- Fixed parameters.
		- Parameters that you set for the model.
	- Free parameters.
		- Parameters that the model learns from the data.
	- Finding coefficients of linear models.
	- **Ax = y** ideally **y** needs to be in the column space of **A**. But typically its not.
	- So we can write the above equation as **Ax + e = y** where **e** is the error vector.


## Day 16 | April 16 2020 | Thursday
Today I continued with matrix spaces and moved on to system of linear equations and matrix determinants.
- Orthogonality, Null spaces and dot-product.
- The four sub-spaces.
- Systems of equations.
	- **Ax = b**.
	- Gaussian Elimination.
		- Matrix Agumentation.
		- Upper diagonal matrix
		- Back-substitution
	- Echelon form.
		- povits of the matrix.
		- Zeros below the pivot.
	- Reduced row Echelon form.
- Matrix Determinants.
	- Only square matrices have a determinant.
	- Determinant is a single number of the matrix.
	- If the determinant of a matrix if **0** then it has linearly dependent columns.
	- Determinant of 3X3 matrix.
		- Agument the same matrix along the right/left verticle axis.
		- From the first matrix take the diagonal elements which might include elements from the agumented matrix.
		- From the second matrix take the off-diagonal elements which might include elements from the matrix which is being used to agument.
	- Finding value of elements from the determinant of the matrix.


## Day 15 | April 15 2020 | Wednesday
Today I kept on learning the matrices and went on understanding about Matrix Rank, Matrix Spaces.
- Rank is defined as dimentionality of information and is given as *r E N, s.t. 0 <= r <= min(m,n) where N = natural numbers, and m,n are the rows and columns of a matrix.*
- Another way of defining the Rank is as *The rank of a matrix is the largest number of columns (or rows) that can form a linearly independent set.*
	- Full row rank matrix
	- Full column rank matrix
	- Full matrix rank
	- Reduced rank
- rank(A) = rank(A<sup>T</sup>) = rank(A<sup>T</sup>A) = rank(AA<sup>T</sup>) *where rank is the function that gives the rank of a matrix*.
- Shifting a matrix by a scaler.	
	-*A* = **A + cI** where **A** is a square matrix, **c** is a constant and **I** is an identity matrix.
- Matrix Spaces.
	- A column space *C(A)* of a matrix **A** is the vector space that is spaned by all of the columns in the matrix doesn't matter if they are linearly independent or linearly dependent.
	- *C(A) = {B<sub>1</sub>a<sub>1</sub> +   + B<sub>n</sub>a<sub>n</sub>}*
	- A row space *R(A) = C(A<sup>T</sup>)* of a matrix **A** is the vector space that is spaned by all the columns in the matrix doesn't matter if they are linearly independent or linearly dependent.
	- Null Spaces *N(A)* of a matrix **A** is the set of all the vectors **{V}** such that **Av = O** and **V != O**.
	- If a matrix has no null space it has linearly independent vectors and vice versa.
	- **A<sup>T</sup>** has the same column space as **A**


## Day 14 | April 14 2020 | Tuesday
Today I started learning about the matrices, notations, terminologies and their operations.
- Types of matrices.
- Trace of the matrix.
- Matrix multiplication.
- Diagonal matrix multplications.
- Consider square matrices **A**, **B** then **(AB)<sup>T</sup>** = **B<sup>T</sup>A<sup>T</sup>**.
- Column weighted multiplication and row weighted multiplication.
- Multiplicative Identity and Additive Identity.
- Matrix **S** is symetric iff **S = (A+A<sup>T</sup>)/2 and A is NxN matrix**
	- **S = S<sup>T</sup>**


## Day 13 | April 13 2020 | Monday
Today I started the Linear Algebra course and learned the fundamental concepts about the linear algebra. I explored some basic vector operations and learned about different spaces.
- Vocabulary of Linear Algebra and Nomenclature.
	- Row vectors, Column Vectors, heads, tails and  Dimensions of the vectors.
- Importance of Linear Algebra and Area of applications.
- Vectors are ordered list of numbers or functions.
- Geometeric interpretation of vectors.
- Vectors subtraction and addition.
	- Dimension needs to be the same.
	- Geometeric Interpretation of operations.
- Scaler multiplication.
	- Magnitude and direction of vector after scaler multiplication.
- Dot product of vectors.
	- A<sub>m<sub>x</sub>n</sub><sup>T</sup> . B<sub>pxq</sub> gives us R<sub>mxq</sub>
	- For dot product to occur **x** and **p** needs to be equal in both matrices.
	- DotProduct = ||A||.||B|| . Cos(angle_between_A_and_B)
	- Law of cosine.
	- Dot product is commutative.
- Magnitude/Norm of vector.
	- || V || = Square_root (V<sup>T</sup>V)
	- Pythagoras theorm.
- Hadamard multiplication or element wise multiplication.
- Outer product ==> V<sub>mxn</sub>.W<sub>pxq</sub><sup>T</sup> ==> R<sub>mxp</sub> (this is the difference between dot product and outer product).
- Complex Number vectors.
	- Complex Number multiplication.
- Harmitian Transpose (a.k.a. conjugate transpose).
- Unit vectors.
- Dimensions and Fields.
- Subspace and Ambient space.
	- Subspace ==> Linear combination ==> Scaler multiplication and addition.
	- Subspace must be closed under addition and/or scaler multiplication.
	- Contains the ZERO vector.
- Ambient space is a higher dimentional space in which sub-spaces lie.
- Span is all possible linear combinations of the vectors in the set.
- Linearly Independent set of vectors is a set in which no vector can be generated by the linaer combination of other vectors.
- Linearly dependent if **O** = C<sub>1</sub>V<sub>1</sub> + C<sub>2</sub>V<sub>2</sub>  + C<sub>3</sub>V<sub>3</sub>   C<sub>n</sub>V<sub>n</sub>  where C is element of **R** and C != 0.
	- That is if the any linear combination of the vectors creates the ZERO vector.
- Basis Vectors.
	- Dimensionality reduction.

## Day 12 | April 12 2020 | Sunday
Today I started learning Anomaly detection problem and Recommendation systems and finally completed the course on Machine learning.
- Anomaly detection.
	- Normal Distribution parameterized with mean and std.
	- Each feature contributes its Normal density function in order to detect anomalies.
	- Don't use anomalies in your training data.
	- Anomaly detection evaluation.
		- Precision Recall
		- F<sub>1</sub>-Score
		- Confussion matrix
	- Anomaly detection vs Supervised Learning.
	- Feature selection in Anomaly detection.
		- Check the distribution of your data if its Normal distribution then its an important feature. (use visualization of data)
		- Try to transform features with non-normal distribution into normal distribution using some transformation function.
		- Feature Engineering.
		- Get more feature or generate new features
	- Multivariate Gaussian (normal) Distribution.
		- Using covariance matrix to change the distribution of the features.
		- Changing the mean of the feature distribution.
		- Can be computationally expensive.
- Recommendation Systems.
	- Motivation for recommendation systems.
	- Feature vectors for data.
	- Weight vector for each user for recommendation.
	- Collaborative filtering.
		- Learn features and their values for the data, from the user preferences.
		- Iterative back and forth learning of weight vectors and feature vectors.
		- Vectorized implementation of collaborative filtering.
		- Mean normalization.
- Large Scale Machine Learning.
	- Always do a sanity check for large datasets by using a smaller dataset.
		- See if it has a lot more variance to capture or it just has captured all the variance of the data and furhter data is not improving anymore. Then we might not need to train the data on full dataset.
	- Use stochastic gradient descent for large datasets to improve from every single exmple.
	- Shaffle the datasets for using stochastic nature optimizers
	- Mini-batch gradient descent.
	- Continous monitering of cost function if its decreasing or not.
	- Online learning as the data stream is comming in your model starts to learn.
	- Parallelsim and MapReduce.
- Machine Learning Pipelines.
	- Measuring accuracy of each step of the pipeline.
	- Accuracy of the pipeline steps can affect the model accuracy.


## Day 11 | April 11 2020 | Saturday
Today I started unsupervised machine learning and learned about the clustering and dimensionality reduction.
- k-Means clustering.
	- Cluster assignment (K = number of clusters)
	- Cluster movement
	- Objective function for K-Means clustering
	- Local Optimal points in K-Means Clustering
		- Try iterative run of K-Means algorithm using random initializations
		- Caculate the distortion of the clusters with the points
		- Pick the best point
	- Chosing the number of clusters
		- Visualize the data.
		- Elbow method using the distortion
- Dimentionality Reduction.
	- Data Compression
	- Data visualization
	- Speed-up machine learning algorithms and reduces the required computation
	- Converts highly corelated features (with almost linear relationship) to a single feature using projection.
	- Projection of higher dimensional data to lower dimensional data (e.g. R<sup>n</sup> ==> R<sup>n-1</sup> ==> R<sup>n-2</sup>  )
- Principal Component Analysis (PCA).
	- Calculates a lower dimensional space for higher dimentional data, such that the squared distances of the data points are small with the calculated lower dimentional space (reduces the projection error).
	- Always perform feature scaling while using PCA (mostly mean normalization is used).
	- Eigen vectors of Covariance vectors of the features of the data.
	- Caculate the eigen vectors from covariance matrix and multiply it with the data keeping the K components (K = [1,2   n]).
	- The more the varaince you are able to capture in lower dimensions the better (best case upto 99%).
	- Reconstruction from the compressed data to original data.
- Using PCA to reduce overfitting is a bad idea although might work okay but it would be better to use regularization to overcome the overfitting, Since PCA through aways some of the variance/information of the data.
	

## Day 10 | April 10 2020 | Friday
Today I started learning the Support Vector Machines.
- Cost function for support vector machines.
	- Essentially the cost funciont adjusts itself such that the decision boundary gets wider using the margins.
	- These margins grow from either side of the boundary equally.
	- Intuitive understanding of why only support vectors contributes in the decision boundary of the support vector machine.
- Kernal functions.
	- Calculation new features using the landmarks.
	- Type of kernal functions.
		- Polynomial kernal (x<sup>T</sup>.l + constant)<sup>degree</sup>.
			- Used very rarely.
		- Linear kernal.
		- Gaussian kernal.
		- String kernal (if the input data is text).
		- chi-square kernal
		- histogram kernal.
		- Intersection kernal.
- SVM in practice.
	- When using Gaussian Kernal do perform feature scaling.
	- Multi-class classification SVMs


## Day 09 | April 09 2020 | Thursday
Today I started learning the common mistakes that people make while improving the machine leraning model.
- Machine Learning Diagnostic.
- Lower dimensional hypothesis functions can be plotted to check them.
- Splitting data in Training, Validation and test set.
- R<sup>2</sup> , Plotting regression error function.
- Percision, Recall, F1-score, AUC-ROC and Accuracy.
	- Precision Recall Trade off.
		- Increasing or decreasing the confidence of the estimator for postive class.
- Bias & Variance analysis.
	- Plotting training and validation error.
	- Bias occurs when the training and validation errors are colse to each other but also are very high.
	- Variance occurs when the training and validation error has a large difference and the training error is very low where as the validation error is very high.
- Regularization overcomes overfitting problem by penalizing the coefficients of the features.
	- Larger value of regularization can introduce higher bias.
	- Smaller value of regularization can introduce higher variance.
- Learning curves.
	- Training error vs Cross validation error.
- Fixes for models.
	- Get more training examples (fixes high variance).
	- Try smaller set of fetures (fixes high variance, but the model might loss some important information).
	- Using lower polynomials (fixes the high variance).
	- Using higher regularization term (fixed the high variance).
	- **Using more data don't actually fixes the high bias problem**.
	- Add more features (fixes the high bias problem).
	- Using higher polynomials (fixes the high bias problem).
	- Using smaller regularization term (fixes high bias problem).
- Machine Learning System desgins.
	- Take some manual look at what errors you model is making.
	- Try to visualize the overall results of your machine learning model against the input.
	- Numerical interpretation of your model, results and data.


## Day 08 | April 08 2020 | Wednesday
Today I continues with neural networks from backpropogation to onword.
- Summing the error over all the output units for the total error of the network.
- Gradient Checking.
- Finally Wrapped my head arround back-propogation

## Day 07 | April 07 2020 | Tuesday
Today I continued with the neural netowrks 
- Some Important links.
	- [ANNs](https://brilliant.org/wiki/artificial-neural-network/)
	- [Feedforward Networks](https://brilliant.org/wiki/feedforward-neural-networks/#formal-definition)
	- [Backpropogation](https://brilliant.org/wiki/backpropagation/)
	- [Neural Networks from scratch](http://neuralnetworksanddeeplearning.com) 
	- [Partial Derivatives](https://brilliant.org/wiki/partial-derivatives/)
- Multiclass classification neural networks output [N,1] dimensional vector where N is number of classes.
- Cost function for neural networks (sigmoid)
- Back propogation Handwritten Execution

## Day 06 | Aprit 06 2020 | Monday
Today I started learning neural networks from scratch.
- History of Neural Networks and anology with brain
- Seeing through your [tongue](https://www.youtube.com/watch?v=48evjcN73rw)!
- A single neuron is a linear classifier
- Concepts of Layers (Input, hidden, output)
- Forward propagation
- Neural Networks for multi-class classification


## Weekend Hacks&Techs | April 04-2020 / April 05-2020 | Saturday & Sunday
For weekend Hacks&Techs I started Pyspark for big data
-PySpark is the Python API written in python to support Apache Spark. Apache Spark is a distributed framework that can handle Big Data analysis
- Big Data is generally greater than or equal to 100GB in size
- Single/Local Machine vs Distributed Systems

|Local/Single Machine |Distributed Systems|
|-----|-----|
|A single machine like your personal computer|A distributed system is a system whose components are located on different networked computers, which communicate and coordinate their actions by passing messages to one another|
|Local machine will use computation resources of a single machine|A distributed system has access to the computational resouces across a number of machines connected through a network|
|Very difficult or some times impossible to scale | Easily scalable by adding as many machines to the network as you want|
|Not fault tolerant, if your machine goes down your process is lost|They also include fault tolerance, if one machine fails, the whole network can still go on|
|Time consumption is very high| You can reduce the time consumption by adding more machines to the network|
- Pyspark setup [instructions](https://github.com/mohsin-ashraf/personal-msds-1/wiki/Spark-setup-on-AWS-EC2)
- Amazon EMR (Elastic Map Reduce)
	- One master node
	- Rest are core nodes
	- Access/Security group settings with IPs
- Spark DataFrames
	- [Important links for Pyspark](https://spark.apache.org/docs/)
		- Select the version and read the documentation
	- To work with PySpark DataFrames we have to use SparkSession
	- PySpark DataFrames
		- DataFrame SQL queries filteration
		- DataFrame basics
		- DataFrame basic operations
		- DataFrame Groupby and Aggregates
		- DataFrame Missing Data
		- Dates and Timestamp
	- Final DataFrame Project
		- Revised all the previous concepts and applied new techniques.
- Spark MLlib
	- Spark MLlib needs the data in a different format. You need to use **Vectors** and **VectorAssembler**
	- PySpark Pipeline
	- PySpark Linear Regression
	- PySpark Logistic Regression
	- PySpark Decision Trees
	- PySpark Random Forests
	- PySpark KMeans Clustering
	- Recommender Systems
		- Content Based
			- A Content-based recommendation system tries to recommend items to users based on their profile. The user's profile revolves around that user's preferences and tastes
		- Colaborative Filtering
			- Recommends based on the knowledge of users' attitude to items, that is, it uses the **wisdom of the crowd** to recommend items 
		- PySpark ALS Recommendation algorithm
	- Natural Language Processing using PySpark
		- CountVectorizer
		- IDF
		- Hash_TF
		- Tokenizer & RegexTokenizer
		- StringIndexer
	- Pyspark Streaming


## Day 05 | April 05 2020 | Sunday
Today I continued with weekend **#Hacks&Techs**. I also learned about the model evaluation methods in detail.
- [Regression Evaluation](https://stats.stackexchange.com/questions/89239/evaluating-a-regression-model/221311#221311?s=a757f4a4fb7a40c7a7f7d53527ac628a)
- [Classification Evaluation](https://web.archive.org/web/20150826060649/http://webdocs.cs.ualberta.ca:80/~eisner/measures.html)
- [AUC - ROC curve](https://towardsdatascience.com/understanding-auc-roc-curve-68b2303cc9c5) is used in binary classification.
	- [Another link](https://www.dataschool.io/roc-curves-and-auc-explained/)

## Day 04 | April 04 2020 | Saturday
Today I started coding Gradient Descent and implemented a very simple Gradient Descent algorithm. I did exercises using Linear Regression and uploaded the code on codebase. I also worked on Weekend **#Hacks&Techs** and did the boilerplate setup.
- implementation of Simplest Gradient Descent Algorithm.
- Predicting house prices using Linear Regression Single Feature.
- Predicting house prices using Linear Regression Single Feature Polynomial Regression.
- Predicting house prices using Linear Regression Multiple Features.
- Predicting house prices using Linear Regression Multiple Features Polynomial Regression.
- Predicting house price using Ridge Regression Multiple Features Polynomial Regression.
- Predicting house price using Lasso Regression Multiple Features Polynomial Regression.


## Day 03 | April 03 2020 | Friday
Today I started learning binary/multi class classification using Logistic Regression. I also learned about the Regularization and its advantages. 
- Sigmoid Function.
- Probabilistic interpretation of sigmoid function.
- Multiple Feature Logistic Regression weights.
	- Finding weights via graphical representation of the data (for atmost 2D data).
	- Finding weights via algebric method.
- Decision boundary
	- Decision boundary is the property of hypothesis function.
	- Multiple Feature, Polynomial Logistic Regression can even make complex circular decision boundaries.
- Logrithmic Cost function for Logistic Regression.
- Applying Gradient Decent on Logistic Regression.
- Advanced Optimization Algorithms.
	- Conjugate Gradient
	- BFGS (Broyden–Fletcher–Goldfarb–Shanno)
	- L-BFGS (L-Broyden–Fletcher–Goldfarb–Shanno)
	- Advantages of these Advanced Optimization Algorithms.
		- No need to manually tune **α**.
		- Often faster than Gradient Descent.
	- Dis-advantages of these Advanced Optimization Algorithms.
		- More complex than Grandient Descent.
- Multiclass Logistic Regression.
	- Combination of binary class Logistic Regressor classifiers for multiclass classification.
- Overfitting:
	- Overfitting occurs when a machine learning model fits the training data very well , but fails to generalize to new examples.
- Regularization is used to stop overfitting.
	- Mathematical intuition of Regularization.
	- Types of Regularization.
		- l1 Regularization (Lasso)
			- It penalizes the coefficients of the features such that, those coefficients exactly become zero. This type of regularization help us in feature selection. 
		- l2 Regularization (Ridge)
			- It reduces the coefficients of the features but don't make them exactly zero.
	- Regularization in Gradient Descent.
	- Regularization in Normal Equation.


## Day 02 | April 02 2020 | Thursday
Today I started digging deeper into the Gradient Descent and started learning maths behind it. I learned about Linear regression with single variable and multiple variable and how Gradient Descent minimizes the cost funciton with high dimensions. Also I refreshed my Linear Algebra concepts for the course.
- Negative & Positive slopes.
- At any minima the slope is 0.
- Linear Algebra.
	- Convex function only have one minima which is global.
	- Matrix scaler operations, Addition and multiplication.
	- Matrix Multiplicaton and its properties.
	- Matrix Inverse and Transpose.
- Linear Regression for Multiple Features.
	- Gradient Descent for multiple features Linear Regression.
	- Gradient Descent converge quickly when features are scaled.
	- Effect of learning rate on convergence.
	- Plotting Cost function to check if the Gradient Descent is working right or not.
	- Polynomial Features (Feature Interactions).
- Linear Regression for Multiple Features Normal Equation.
	- Normal Equation for Linear Regression .
	- Feature Scaling is not required.

|Gradient Decent|Normal Equation|
|-----|-----|
|Need to choose Learning Rate **α**|No need to choose Learning Rate **α**|
|Needs many iterations|Don't need to iterate|
|Works well even when **n** (dataset size) is large|Need to perform intensive matrix operations|


	
## Day 01 | April 01 2020 | Wednesday 
- Started Machine Learning Course by Adrew Ng [Coursera].
- Learned what is machine learning and types of Machine Learning.
	- Supervised Learning.
	- Unsupervised Learning.
	- Re-enforcement Learning.
	- Clustering.
	- Cocktail party problem (algorithm).
- Learned the difference between Supervised and Unsupervised Learning.
	- Supervised Learning.
		- Spam Filtering, Perdicting house prices
	- Unsupervised Learning.
		- Customer Segmentation, Article clustering
- Linear Regression.
- Machine Learning Glossary.
	- Features
	- Labels
	- Hypothesis function	
	- Cost functions 
	- Cost function
	- Contour plots for cost funtions.
	- Gradient Descent.
	- Learning Rate.