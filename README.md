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
    - [afterAll (.ts only)](#afterall-ts-only)
    - [afterEach (.ts only)](#aftereach-ts-only)
    - [beforeAll (.ts only)](#beforeall-ts-only)
    - [beforeEach (.ts only)](#beforeeach-ts-only)
    - [describe (.ts only)](#describe-ts-only)
    - [expect (.ts only)](#expect-ts-only)
    - [fdescribe (.ts only)](#fdescribe-ts-only)
    - [fit (.ts only)](#fit-ts-only)
    - [it (.ts only)](#it-ts-only)
    - [pending (.ts only)](#pending-ts-only)
    - [spyOn (.ts only)](#spyon-ts-only)
    - [xdescribe (.ts only)](#xdescribe-ts-only)
    - [xit (.ts only)](#xit-ts-only)
  - [Matchers](#matchers)
    - [nothing (.ts only)](#nothing-ts-only)
    - [toBe (.ts only)](#tobe-ts-only)
    - [toBeCloseTo (.ts only)](#tobecloseto-ts-only)
    - [toBeCloseTo (with precision) (.ts only)](#tobecloseto-with-precision-ts-only)
    - [toBeDefined (.ts only)](#tobedefined-ts-only)
    - [toBeFalsy (.ts only)](#tobefalsy-ts-only)
    - [toBeGreaterThan (.ts only)](#tobegreaterthan-ts-only)
    - [toBeGreaterThanOrEqual (.ts only)](#tobegreaterthanorequal-ts-only)
    - [toBeLessThan (.ts only)](#tobelessthan-ts-only)
    - [toBeLessThanOrEqual (.ts only)](#tobelessthanorequal-ts-only)
    - [toBeNan (.ts only)](#tobenan-ts-only)
    - [toBeNegativeInfinity (.ts only)](#tobenegativeinfinity-ts-only)
    - [toBeNull (.ts only)](#tobenull-ts-only)
    - [toBePositiveInfinity (.ts only)](#tobepositiveinfinity-ts-only)
    - [toBeTruthy (.ts only)](#tobetruthy-ts-only)
    - [toBeUndefined (.ts only)](#tobeundefined-ts-only)
    - [toContain (.ts only)](#tocontain-ts-only)
    - [toEqual (.ts only)](#toequal-ts-only)
    - [toHaveBeenCalled (.ts only)](#tohavebeencalled-ts-only)
    - [toHaveBeenCalledBefore (.ts only)](#tohavebeencalledbefore-ts-only)
    - [toHaveBeenCalledTimes (.ts only)](#tohavebeencalledtimes-ts-only)
    - [toHaveBeenCalledWith (.ts only)](#tohavebeencalledwith-ts-only)
    - [toMatch (.ts only)](#tomatch-ts-only)
  - [Spys](#spys)
    - [createSpy (.ts only)](#createspy-ts-only)
    - [createSpyObj (.ts only)](#createspyobj-ts-only)
    - [and.callFake (.ts only)](#andcallfake-ts-only)
    - [and.callThrough (.ts only)](#andcallthrough-ts-only)
    - [and.returnValue (.ts only)](#andreturnvalue-ts-only)
    - [and.returnValues (.ts only)](#andreturnvalues-ts-only)
    - [and.throwError (.ts only)](#andthrowerror-ts-only)

<!-- TOC END -->

# Install

`apm install jasmine-snippets`

# Supported languages

- [ ] JavaScript
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

- JavaScript
- Python
- Ruby
- [TypeScript](https://github.com/guilhermejcgois/atom-jasmine-snippets/blob/master/snippets/typescript.cson)

### afterAll (.ts only)
```
afterAll
```

### afterEach (.ts only)
```
afterEach
```

### beforeAll (.ts only)
```
beforeAll
```

### beforeEach (.ts only)
```
beforeEach
```

### describe (.ts only)
```
describe
```

### expect (.ts only)
```
expect
```

### fdescribe (.ts only)
```
fdescribe
```

### fit (.ts only)
```
fit
```

### it (.ts only)
```
it
```

### pending (.ts only)
```
pend
```

### spyOn (.ts only)
```
spyOn
```

### xdescribe (.ts only)
```
xdescribe
```

### xit (.ts only)
```
xit
````

## Matchers

- JavaScript
- Python
- Ruby
- [TypeScript](https://github.com/guilhermejcgois/atom-jasmine-snippets/blob/master/snippets/typescript.matchers.cson)

### nothing (.ts only)
```
exp-n
```

### toBe (.ts only)
```
exp-tb
```

### toBeCloseTo (.ts only)
```
exp-tbct
```

### toBeCloseTo (with precision) (.ts only)
```
exp-tbctp
```

### toBeDefined (.ts only)
```
exp-tbd
```

### toBeFalsy (.ts only)
```
exp-tbf
```

### toBeGreaterThan (.ts only)
```
exp-tbgt
```

### toBeGreaterThanOrEqual (.ts only)
```
exp-tbgtoe
```

### toBeLessThan (.ts only)
```
exp-tblt
```

### toBeLessThanOrEqual (.ts only)
```
exp-tbltoe
```

### toBeNan (.ts only)
```
exp-nan
```

### toBeNegativeInfinity (.ts only)
```
exp-ninf
```

### toBeNull (.ts only)
```
exp-null
```

### toBePositiveInfinity (.ts only)
```
exp-inf
```

### toBeTruthy (.ts only)
```
exp-tbt
```

### toBeUndefined (.ts only)
```
exp-tbud
```

### toContain (.ts only)
```
exp-tc
```

### toEqual (.ts only)
```
exp-teq
```

### toHaveBeenCalled (.ts only)
```
exp-thbc
```

### toHaveBeenCalledBefore (.ts only)
```
exp-thbcb
```

### toHaveBeenCalledTimes (.ts only)
```
exp-thbct
```

### toHaveBeenCalledWith (.ts only)
```
exp-thbcw
```

### toMatch (.ts only)
```
exp-tm
```

## Spys

- JavaScript
- Python
- Ruby
- [TypeScript](https://github.com/guilhermejcgois/atom-jasmine-snippets/blob/master/snippets/typescript.spys.cson)

### createSpy (.ts only)
```
jasm-spy
```

### createSpyObj (.ts only)
```
jasm-spyobj  // for only one method
jasm-spyobjs // for multiple methods
```

### and.callFake (.ts only)
```
jasm-fake
```

### and.callThrough (.ts only)
```
jasm-through
```

### and.returnValue (.ts only)
```
jasm-retValue
```

### and.returnValues (.ts only)
```
jasm-retValues
```

### and.throwError (.ts only)
```
jasm-error
```
