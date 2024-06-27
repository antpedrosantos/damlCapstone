
# LibraryAccountProject
LibraryAccountProject is a project management application built in Daml.

### I. Overview 
This project was created by using the `empty-skeleton` template. The project adopts and exemplifies the `proposal-accept` design pattern. 

Student can create a StudentRequest contract. Librarian can either Reject or Approve the request. Upon getting rejected, student can exercise Revise to re-propose the project with updated details. Upon getting approved, a StudentAccount contract is created.


### II. Workflow
  1. student creates a StudentRequest contract  
  2. student cancels request   
  3. librarian exercises Reject with a feedback: "Revise email"
  4. student exercises Revise with amended e-mail
  5. librarian exercises Approve - a StudentAccount contract is created

### III. Challenge(s)
* The project was created by using `empty-skeleton` and the following was added to `daml.yaml`:

exposed-modules:
  - Main
```
For more info, check out [this post](https://discuss.daml.com/t/sandbox-options-wall-clock-time/5692/16?u=cathy_jung) on Daml Forum and [Daml Doc](https://docs.daml.com/tools/navigator/index.html?&_ga=2.48248804.337210607.1673989679-241632404.1672853064&_gac=1.17025355.1673455980.CjwKCAiA2fmdBhBpEiwA4CcHzfI2w1_D95zAr3_d6QTypOMXGTpUxtS06c55inucNwZvUZn4AebsJxoCZEgQAvD_BwE&_gl=1*elem6v*_ga*MjQxNjMyNDA0LjE2NzI4NTMwNjQ.*_ga_GVK9ZHZSMR*MTY3Mzk5NDQzOS4zMS4xLjE2NzM5OTQ3MDcuMC4wLjA.#logging-in-as-a-party).


### IV. Compiling & Testing
To compile and test, run the pre-written script in the `Test.daml` under /daml OR run:
```
$ daml start
```
