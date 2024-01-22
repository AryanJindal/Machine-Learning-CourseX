# Batch Machine Learing | Offline vs Online | MAchine learning types

## How ML models are trained on production

**Production** It is the server on which our code i going to run

## Batch Learing | Offline

- Process
- ![Batch](./Batch%20Learning.png)
- **problem** the model is static, for exaple market trends continues to change , same with the taste of the user. So the model is requierd to keep itself updated.
- **Solution**   every 24hr or week , retrain the model
    1) Bring the new Data
    2) Merge with old one
    3) retrain the model
    4) Deploy to the server.

- **Disadvantages**
  - Huge data
  - hardware limitation
  - Availability(Suppose a software deployed with military and now ,they got off the grid.)
  - Secondly, suppose model updates every 24hr, but we have important info to send to users or train the model. Then , it wont be possible instantenously and our model will have lag.
  
