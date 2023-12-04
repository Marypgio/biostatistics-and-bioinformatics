# biostatistics-and-bioinformatics
This was part of an assingnment for my PG cert Bioistatistics and Bioinformatics course.

The code defines a Python function eutos_score that calculates a patient's EUTOS score based on two inputs: their basophil percentage and spleen size. The EUTOS score is a risk assessment tool that categorizes patients into low-risk and high-risk groups.
The function first checks if the inputs provided are within the specified ranges (basophil percentage in the range 0-25 and spleen size in the range 0-40) using try and except statements for error handling in case of incorrect input types.
Once the inputs are validated, the EUTOS score is calculated using the formula (7 x basophil [%]) + (4 x spleen [cm]).
If the resulting score is greater than 87, the patient is classified as high-risk, and the function returns 'High risk' along with the patient's score. If the score is less than or equal to 87, the patient is classified as low-risk, and the function returns 'Low risk' along with the patient's score.
 
The max() and min() functions are used to make sure that the inputs are within the specified ranges. If the input is less than 0, it will be set to 0, and if it's greater than the maximum value, it will be set to the maximum value.

The final patient score is calculated by multiplying the basophil percentage by 7 (as specified in the EUTOS scoring system), multiplying the spleen size by 4 (also specified in the system), and adding the two numbers together.

The try...except block is used to handle errors that may occur if the inputs are not numeric. If the input is not numeric, the function will return the message 'Invalid input'.

Testing:
To test the function, we can call it with sample inputs, the user can call the function with different customized numbers, for example:
# Calling the function with basophil percentage = 15 and spleen size = 35
# Example of output 'High risk'
result = eutos_score(15, 35)

# Printing the result returned by the function

print(result)
('High risk', 245)

# Calling the function with basophil percentage = 5 and spleen size = 10
# Example of output 'Low risk'
result = eutos_score(5, 10)

# Printing the result returned by the function
print(result)
('Low risk', 75)






print(result)
