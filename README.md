| Travis CI | npm |
| :-: | :-: |
| [![Build Status](https://travis-ci.org/dperuo/riker-ipsum.svg?branch=master)](https://travis-ci.org/dperuo/riker-ipsum) | [![npm version](https://badge.fury.io/js/riker-ipsum.svg)](http://badge.fury.io/js/riker-ipsum) |

# Code Challenge for General Assembly

## Quick Start

```bash
cd path/to/folder
npm install
python -m SimpleHTTPServer 9876 & open http://localhost:9876/
```

This application defaults to port 9876 on localhost. You can specify a different port by replacing `9876` in the code above with the port of your choice.

## Unit Tests

[Karma][karma] is used for unit testing. Run the karma spec from the command line:

[karma]: https://karma-runner.github.io/0.13/index.html

```bash
cd path/to/folder
npm test
```

The Karma configuration launches Chrome by default. You can launch a different browser by updating the `browsers` array in `karma.conf.js` with the [browsers of your choice][browsers].

[browsers]: https://karma-runner.github.io/0.13/config/browsers.html

## Task

* Please write a program that:

  * Assembles a collection of student records by parsing data from 3 different files
  * Displays the collection 3 times, sorted 3 different ways

* What we're looking for here is clear code and elegant object-oriented design. Please avoid imperative or functional coding style, or an overly clever solution.

* When finished, please package and submit your solution as an email attachment. (Please do **not** publish your code anywhere!) Send the email to code-challenge@generalassemb.ly with instructions on how to run your program

### Criteria

The qualities we're looking for are:

  * **Clarity**: is the intent of the code obvious? Are things named appropriately?
  * **Maintainability:**: how flexible is the code?
  * **Testability**: is it easy to test the code? _Please demonstrate with unit tests._

### Input

Please copy the data files (in the `data` folder) and include them in your solution.

  * comma.txt
    * Delimiter: `,`
    * Order: `last_name`, `first_name`, `campus`, `favorite_color`, `date_of_birth`

  * dollar.txt
    * Delimiter: `$`
    * Order: `last_name`, `first_name`, `middle_initial`, `campus`, `date_of_birth`, `favorite_color`

  * pipe.txt
    * Delimiter: `|`
    * Order: `last_name`, `first_name`, `middle_initial`, `campus`, `favorite_color`, `date_of_birth`

### Output

Please display the collection in three different ways:

  1. Sorted by `campus` (ascending), then by `last_name` (ascending)
  2. Sorted by `date_of_birth` (ascending)
  3. Sorted by `last_name` (descending)

Below is the expected output:

```
Output 1:
Kirlin Mckayla Atlanta 5/29/1986 Maroon
Barrows Anika Hong Kong 5/5/1965 Spring Green
Goyette Timmothy London 10/2/1964 Pacific Blue
Nolan Rhiannon Los Angeles 10/4/1974 Vivid Tangerine
Parker Matteo Melbourne 2/14/1962 Burnt Sienna
Bednar Filomena New York City 1/24/1980 Salmon
Cummerata Elliot New York City 4/3/1947 Neon Carrot
Wilkinson Stacy New York City 1/22/1964 Shocking Pink
Bruen Rigoberto San Francisco 12/1/1962 Raw Umber

Output 2:
Cummerata Elliot New York City 4/3/1947 Neon Carrot
Parker Matteo Melbourne 2/14/1962 Burnt Sienna
Bruen Rigoberto San Francisco 12/1/1962 Raw Umber
Wilkinson Stacy New York City 1/22/1964 Shocking Pink
Goyette Timmothy London 10/2/1964 Pacific Blue
Barrows Anika Hong Kong 5/5/1965 Spring Green
Nolan Rhiannon Los Angeles 10/4/1974 Vivid Tangerine
Bednar Filomena New York City 1/24/1980 Salmon
Kirlin Mckayla Atlanta 5/29/1986 Maroon

Output 3:
Wilkinson Stacy New York City 1/22/1964 Shocking Pink
Parker Matteo Melbourne 2/14/1962 Burnt Sienna
Nolan Rhiannon Los Angeles 10/4/1974 Vivid Tangerine
Kirlin Mckayla Atlanta 5/29/1986 Maroon
Goyette Timmothy London 10/2/1964 Pacific Blue
Cummerata Elliot New York City 4/3/1947 Neon Carrot
Bruen Rigoberto San Francisco 12/1/1962 Raw Umber
Bednar Filomena New York City 1/24/1980 Salmon
Barrows Anika Hong Kong 5/5/1965 Spring Green
```
