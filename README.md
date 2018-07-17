This is a runnable example to demonstrate [testdouble/teenytest#38](https://github.com/testdouble/teenytest/issues/#38).

## Running this

To run this, clone this gist, install dependencies, and run the tests with `npm test`

```shell
git clone https://github.com/amiel/teenytest-glob-issue
cd teenytest-glob-issue
npm install
npm test
```

## Expected result

I expected teenytest to run both `example-1.test.js` and `example_2.test.js`.


## Actual Result

With these files, teenytest only runs `example_2.test.js`, and not
`example-1.test.js`.


```

> teenytest-glob-issue-example@0.0.0 test /Users/amiel/src/experiments/teenytest-glob
> teenytest test/**/*.test.js

TAP version 13
1..1
ok 1 - test #1 in `test/lib/example_2.test.js`
# Test run passed!
#   Passed: 1
#   Failed: 0
#   Total:  1
```

