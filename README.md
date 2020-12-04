# SVM-with-Keras
Building Recognition at ITB

This algorthim doesn't need SVC classfier from library sklearn.svm. It use library from Keras.
In classifier, we need squared hinge and regularizer to complete SVM's loss function. Therefore, on the last layer, I placed regularization parameter before code activation

Source of this algorithm:
<ul>
  <li>https://medium.com/nybles/create-your-first-image-recognition-classifier-using-cnn-keras-and-tensorflow-backend-6eaab98d14dd</li>
  <li>https://stackoverflow.com/questions/54414392/convert-sklearn-svm-svc-classifier-to-keras-implementation</li>
</ul>

With the following modifications:
<ul>
  <li>Placed linear activation function in the last layer before using l2 regularization</li>
  <li>Didn't use mode.fit function and changed it with model.fit_generator to use epoch funtion. In this code, model variabel named classifier</li>
  <li>Used abs and np.mean function on "nilai" variable to get better value</li>
</ul>
