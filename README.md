# Jasmine snippets for Atom

This is a collection of jasmine statements common in my day by day.

Found some typo? Miss something else cool? Let me now or make a pull request!

<!-- TOC -->
- [Install](#install)
- [Supported languages](#supported-languages)
- [Snippets](#snippets)
  - [Custom](#custom)
    - [custom_equality (.ts only)](#custom_equality-ts-only)
    - [custom_matcher (.ts only)](#custom_matcher-ts-only)
  - [Globals](#globals)
    - [afterAll (.js and .ts only)](#afterall-ts-only)
    - [afterEach (.js and .ts only)](#aftereach-ts-only)
    - [beforeAll (.js and .ts only)](#beforeall-ts-only)
    - [beforeEach (.js and .ts only)](#beforeeach-ts-only)
    - [describe (.js and .ts only)](#describe-ts-only)
    - [expect (.js and .ts only)](#expect-ts-only)
    - [fdescribe (.js and .ts only)](#fdescribe-ts-only)
    - [fit (.js and .ts only)](#fit-ts-only)
    - [it (.js and .ts only)](#it-ts-only)
    - [pending (.js and .ts only)](#pending-ts-only)
    - [spyOn (.js and .ts only)](#spyon-ts-only)
    - [xdescribe (.js and .ts only)](#xdescribe-ts-only)
    - [xit (.js and .ts only)](#xit-ts-only)
  - [Matchers](#matchers)
    - [nothing (.js and .ts only)](#nothing-ts-only)
    - [toBe (.js and .ts only)](#tobe-ts-only)
    - [toBeCloseTo (.js and .ts only)](#tobecloseto-ts-only)
    - [toBeCloseTo (with precision) (.js and .ts only)](#tobecloseto-with-precision-ts-only)
    - [toBeDefined (.js and .ts only)](#tobedefined-ts-only)
    - [toBeFalsy (.js and .ts only)](#tobefalsy-ts-only)
    - [toBeGreaterThan (.js and .ts only)](#tobegreaterthan-ts-only)
    - [toBeGreaterThanOrEqual (.js and .ts only)](#tobegreaterthanorequal-ts-only)
    - [toBeLessThan (.js and .ts only)](#tobelessthan-ts-only)
    - [toBeLessThanOrEqual (.js and .ts only)](#tobelessthanorequal-ts-only)
    - [toBeNan (.js and .ts only)](#tobenan-ts-only)
    - [toBeNegativeInfinity (.js and .ts only)](#tobenegativeinfinity-ts-only)
    - [toBeNull (.js and .ts only)](#tobenull-ts-only)
    - [toBePositiveInfinity (.js and .ts only)](#tobepositiveinfinity-ts-only)
    - [toBeTruthy (.js and .ts only)](#tobetruthy-ts-only)
    - [toBeUndefined (.js and .ts only)](#tobeundefined-ts-only)
    - [toContain (.js and .ts only)](#tocontain-ts-only)
    - [toEqual (.js and .ts only)](#toequal-ts-only)
    - [toHaveBeenCalled (.js and .ts only)](#tohavebeencalled-ts-only)
    - [toHaveBeenCalledBefore (.js and .ts only)](#tohavebeencalledbefore-ts-only)
    - [toHaveBeenCalledTimes (.js and .ts only)](#tohavebeencalledtimes-ts-only)
    - [toHaveBeenCalledWith (.js and .ts only)](#tohavebeencalledwith-ts-only)
    - [toMatch (.js and .ts only)](#tomatch-ts-only)
  - [Spys](#spys)
    - [createSpy (.js and .ts only)](#createspy-ts-only)
    - [createSpyObj (.js and .ts only)](#createspyobj-ts-only)
    - [and.callFake (.js and .ts only)](#andcallfake-ts-only)
    - [and.callThrough (.js and .ts only)](#andcallthrough-ts-only)
    - [and.returnValue (.js and .ts only)](#andreturnvalue-ts-only)
    - [and.returnValues (.js and .ts only)](#andreturnvalues-ts-only)
    - [and.throwError (.js and .ts only)](#andthrowerror-ts-only)

<!-- TOC END -->

# Install

`apm install jasmine-snippets`

# Supported languages

- [x] JavaScript
- [ ] Python
- [ ] Ruby
- [x] TypeScript

# Snippets

Below I list all the available snippet's prefix. I'm not will cover what they produces, 'cause will only be a copy-paste from .cson files.

## Custom

- JavaScript
- Python
- Ruby
- [TypeScript](https://github.com/guilhermejcgois/atom-jasmine-snippets/blob/master/snippets/typescript.custom.cson)

### custom_equality (.ts only)
```
var myCustomEquality = function(first, second) {
  // return true or false if first and second are comparable,
  // otherwise, doesn't return nothig.
};

beforeEach(function () {
  jasmine.addCustomEqualityTester(myCustomEquality);
});
```

### custom_matcher (.ts only)
```
var customMatchers = {
  toBeCompared: function (util, curstomEqualityTester) {
    return  {
      compare: function (actual, expected) {
        ...[negative]C[negative]C
        var result = {};

        // Assign result.pass to true or false, and result.message to some string

        return result;
      }
    }
  };
  ...
};

beforeEach(function () {
  jasmine.addCustomEqualityTester(customMatchers);
});
```

## Globals

- [JavaScript](https://github.com/guilhermejcgois/atom-jasmine-snippets/blob/master/snippets/JavaScript.cson)
- Python
- Ruby
- [TypeScript](https://github.com/guilhermejcgois/atom-jasmine-snippets/blob/master/snippets/typescript.cson)

### afterAll (.js and .ts only)
```
afterAll
```

### afterEach (.js and .ts only)
```
afterEach
```

### beforeAll (.js and .ts only)
```
beforeAll
```

### beforeEach (.js and .ts only)
```
beforeEach
```

### describe (.js and .ts only)
```
describe
```

### expect (.js and .ts only)
```
expect
```

### fdescribe (.js and .ts only)
```
fdescribe
```

### fit (.js and .ts only)
```
fit
```

### it (.js and .ts only)
```
it
```

### pending (.js and .ts only)
```
pend
```

### spyOn (.js and .ts only)
```
spyOn
```

### xdescribe (.js and .ts only)
```
xdescribe
```

### xit (.js and .ts only)
```
xit
````

## Matchers

- [JavaScript](https://github.com/guilhermejcgois/atom-jasmine-snippets/blob/master/snippets/matchers.cson)
- Python
- Ruby
- [TypeScript](https://github.com/guilhermejcgois/atom-jasmine-snippets/blob/master/snippets/matchers.cson)

### nothing (.js and .ts only)
```
exp-n
```

### toBe (.js and .ts only)
```
exp-tb
```

### toBeCloseTo (.js and .ts only)
```
exp-tbct
```

### toBeCloseTo (with precision) (.js and .ts only)
```
exp-tbctp
```

### toBeDefined (.js and .ts only)
```
exp-tbd
```

### toBeFalsy (.js and .ts only)
```
exp-tbf
```

### toBeGreaterThan (.js and .ts only)
```
exp-tbgt
```

### toBeGreaterThanOrEqual (.js and .ts only)
```
exp-tbgtoe
```

### toBeLessThan (.js and .ts only)
```
exp-tblt
```

### toBeLessThanOrEqual (.js and .ts only)
```
exp-tbltoe
```

### toBeNan (.js and .ts only)
```
exp-nan
```

### toBeNegativeInfinity (.js and .ts only)
```
exp-ninf
```

### toBeNull (.js and .ts only)
```
exp-null
```

### toBePositiveInfinity (.js and .ts only)
```
exp-inf
```

### toBeTruthy (.js and .ts only)
```
exp-tbt
```

### toBeUndefined (.js and .ts only)
```
exp-tbud
```

### toContain (.js and .ts only)
```
exp-tc
```

### toEqual (.js and .ts only)
```
exp-teq
```

### toHaveBeenCalled (.js and .ts only)
```
exp-thbc
```

### toHaveBeenCalledBefore (.js and .ts only)
```
exp-thbcb
```

### toHaveBeenCalledTimes (.js and .ts only)
```
exp-thbct
```

### toHaveBeenCalledWith (.js and .ts only)
```
exp-thbcw
```

### toMatch (.js and .ts only)
```
exp-tm
```

## Spys

- [JavaScript](https://github.com/guilhermejcgois/atom-jasmine-snippets/blob/master/snippets/spys.cson)
- Python
- Ruby
- [TypeScript](https://github.com/guilhermejcgois/atom-jasmine-snippets/blob/master/snippets/spys.cson)

### createSpy (.js and .ts only)
```
jasm-spy
```

### createSpyObj (.js and .ts only)
```
jasm-spyobj  // for only one method
jasm-spyobjs // for multiple methods
```

### and.callFake (.js and .ts only)
```
jasm-fake
```

### and.callThrough (.js and .ts only)
```
jasm-through
```

### and.returnValue (.js and .ts only)
```
jasm-retValue
```

### and.returnValues (.js and .ts only)
```
jasm-retValues
```

### and.throwError (.js and .ts only)
```
jasm-error
```
