# Schedulers
Schedulers are used to perform scheduled tasks.  
Please note don't leave something blank, otherwise it will not be loaded.
### Example 1
Here is a simple scheduler that only performs the task of sending announcements.
```yaml
example-1:
  delay: 10
  actions:
    - "broadcast::Hello there"
    - "broadcast::It is an example announcement"
```
`Delay` is the number of seconds to wait before sending(or running actions).  
`Actions` is a list of strings that will be executed when the scheduler executes(please follow the format written for each string in this list, otherwise it will not be executed).
### Example 2
```yaml
example-2:
  manuallyStart: true
  delay: 10
  actions:
    - "broadcast::Hello there"
    - "broadcast::It is an example announcement.(started scheduler manually)" 
```
`manuallyStart` is a boolean indicating whether you don't want the scheduler to start automatically.
*You can start by execute the command: `/scheduler start example-2`*