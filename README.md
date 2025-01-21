## Install Virtual Env

* We use conda virtaul environments. Documentation here: https://docs.anaconda.com/miniconda/
* conda create --name env python=3.10
* conda activate env
* pip install -r requirements.txt (some of the packages here might not be needed, i merged this list from a prior project that used this env)


## Study Domain: Hungry Thirsty 

<img src="https://user-images.githubusercontent.com/6353393/217291559-d9db4a5c-b1df-4f3f-a2c4-5d26d6c017a7.png" alt="Hungry Thirsty" width="30%">

* We use the Hungry Thirsty domain as a testbed for studying reward design. 
* In Hungry Thirsty, food is located in one random corner; water in another.
* The goal is for the agent to eat as much as possible, but the agent can only eat if it’s not thirsty.
* If the agent drinks, it becomes not thirsty. If the agent doesn’t drink, it becomes thirsty with 10% probability.
* The optimal policy is for the agent to navigate to the water and drink whenever it's thirsty, but to navigate to the food and eat whenever it's not thirsty. 

Inside Domains/gym-hungry-thirsty/, there is a hungry-thirsty-user-control file where you can test out the env.