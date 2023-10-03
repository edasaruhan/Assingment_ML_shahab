#Hw1 - Hw1 - You shouldt use z_score builtin function. You should use equation  of z score
#Hw2 – 
 Step 4: Define the cost function (logistic loss)
def logistic_loss(y_true, y_pred):
    epsilon = 1e-15   # Small constant to avoid log(0)
    y_pred = np.clip(y_pred, epsilon, 1 - epsilon)
    return - (y_true * np.log(y_pred) + (1 - y_true) * np.log(1 - y_pred))
y_true = np.array([1, 0, 1, 0, 1])  # True binary labels
y_pred = np.array([0.9, 0.1, 0.8, 0.2, 0.7])  # Predicted probabilities

 Calculate the logistic loss
loss = logistic_loss(y_true, y_pred)

 result
print("Logistic Loss:", loss)
we dont want to use y_ture and y_pred because we have x_train and y_test from iris dataset.
Thank you for your efforts :)
