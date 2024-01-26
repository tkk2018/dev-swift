# dispatch

## DispatchQueue

The `DispatchQueue.main` is a special (single) thread for UI.

```swift
DispatchQueue.main.async {
}
```

The `DispatchQueue.global` doesn't run in single thread. The max number of thread is based on the CPU core. The system will decide whether want to create a new thread to run the closure.

```swift
DispatchQueue.global.async {
}
```

The `DispatchQueue` created by app is a single thread which will run in sequence (FIFO).

```swift
let dispatch = DispatchQueue()
dispatch.async {
}
```
