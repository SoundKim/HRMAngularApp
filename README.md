### Promise vs Observable
1. Multiple Values:
While Promises are used to represent a single value that will be resolved or rejected in the future, Observables can represent multiple values over time. Observables can emit values continuously, whereas Promises only emit a single value.

2. Cancellation:
Unlike Promises, which cannot be canceled once a request is made, Observables can be canceled using the unsubscribe method. This feature is useful when you no longer need to listen to the events emitted by the Observable.

3. Lazy Execution:
Promises execute immediately when they are created, while Observables are lazy and do not execute until someone subscribes to them. This lazy execution can help to reduce unnecessary computation and increase performance.

4. Composability:
Observables are composable, which means they can be combined to create more complex streams of data. Observables also offer operators like map, filter, and reduce to transform the data emitted by them. Promises, on the other hand, cannot be composed in the same way as Observables.

5. Error Handling: 
Both Promises and Observables allow for error handling, but Observables have additional error handling methods such as .retry() and .retryWhen() that are not available in Promises.
