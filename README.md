# Repro for a potential bug in qunit v2.17.0

## To reproduce:

1. Open `test.html` in a browser
1. Filter for something that doesn't exist in the tests, such as 'cat'
1. See no exception thrown and curious results

## To see node behavior:

1. `npm install`
1. `npx qunit --filter='cat'` 
1. Observe error as expected

## To see v2.16.0 behavior

1. Open `test-2-16.html` in a browser
1. Filter for something that doesn't exist in the tests, such as 'cat'
1. See exception thrown in console, though unfortunate lack of feedback in UI
