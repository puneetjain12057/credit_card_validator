
# Credit Card Validator

A simple C++ program which validates credit card numbers using Luhn's Algorithm.

# Luhn Algorithm

The Luhn algorithm, also known as the modulus 10 or mod 10 algorithm, is a simple checksum formula used to validate a variety of identification numbers, such as credit card numbers, IMEI numbers, Canadian Social Insurance Numbers. Most credit cards and many government identification numbers use the algorithm as a simple method of distinguishing valid numbers from mistyped or otherwise incorrect numbers. It was designed to protect against accidental errors, not malicious attacks.

Step 1 – Starting from the rightmost digit, double the value of every second digit

Step 2 – If doubling of a number results in a two digit number i.e greater than 9(e.g., 6 × 2 = 12), then add the digits of the product (e.g., 12: 1 + 2 = 3, 15: 1 + 5 = 6), to get a single digit number. 

Step 3 – Now take the sum of all the digits.

Step 4 – If the total modulo 10 is equal to 0 (if the total ends in zero) then the number is valid according to the Luhn formula; else it is not valid.


# Docker

Download Docker Desktop for Mac or Windows. Docker Compose will be automatically installed. On Linux, make sure you have the latest version of Compose.

This solution uses GCC to compile the code.

Run the following command to create a image and run it.

Step 1 – Below command is for create an image. 
```bash
docker build -t {image-name}:tag .
```
Step 2 – Below command is for run the image.

```bash
docker run --rm -it {image-name}:tag
```

# kubernetes

First, you need to clone this repository:

```bash
git clone https://github.com/puneetjain12057/credit_card_validator.git
```

Then, change directory to your local copy:

```bash
cd kubernetes
```

Now apply the deployment and service yaml to create a pods and service.

```bash
kubectl apply -f deployment.yaml
```
```bash
kubectl apply -f deployment.yaml
```

Now check if your pods are up and running. Also service is also up with below command.

```bash
kubectl get pods
```

```bash
kubectl get svc
```

Now you can open your browser and put below url in your browser to check if your code is host on localhost or not.

```bash
localhost:8083
```