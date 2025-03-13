# Instructions

1. Clone the repo

```console
git clone https://github.com/david-dxc/DAML-Challenge.git
```

2. Navigate to the project

```console
cd DAML-challenge
```

3. And run

```console
daml start
```

> Note: The scripts are executed all together so prints must be seen in console

# Learning

1. I tried to use a smart contract after i use it(consumed, archived)
   1. after executing the first operation this contract does no longer exist
2. I don't know how to develop several files
3. I dont know how to execute more tahn 1 script per execution
4. The script runs before the project start executing, this must be for testing purposes

## Code

1. `queryContractId` API function that allows to query the details of a contract
   1. signatary
   2. observer
2. `$` Apply the result of the left to the right is better than using ()
3. `createCmd` comes from DAML API, and this is to create an instance of a template
   1. creates a smart contract from scratch
   2. DOESNT REQUIRE AN EXISTING CONTRACT
4. `excerciseCmd` DAML API, executes a choice of an existing contract
   1. can modify the existing contract
   2. can create a new contrat
5. `CreateTask` is a choice only existing inside of template
   1. REQUIRES AN EXISTING CONTRACT
   2. INHERITS MOST OF THE VALUES OF THE ORIGINAL CONTRACT
6. It is also possible to create choice with more than 1 param and optional params
