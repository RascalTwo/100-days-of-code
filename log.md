# 100 Days Of Code - Log

## Day 000: January 1, 2023

- Forked & Cloned this very repo!

## Day 001: January 2, 2023

[igf]: https://github.com/JoeSangine/image-generalization-finder
[together]: https://github.com/Caleb-Cohen/Together

|                                                                  Codewar                                                                  |                                       LeetCode                                        |                                               Quotes                                               |
| :---------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------: |
| [Number of anagrams in an array of words](https://www.codewars.com/kata/reviews/587e18bd7a25e865530000da/groups/63b224cff23f1000018ca98c) | [Detect Capital](https://leetcode.com/problems/detect-capital/submissions/869349756/) | [Up](https://media-quotes.onrender.com/ejs/search?query=I+finally+meet+my+childhood+hero&title=Up) |

- Setup E2E testing via [Cypress](https://www.cypress.io/) with **_FULL_** code coverage reporting on an [OAuth-using MERN application][together].
  - Tried using more lower-level modules such as [`node-request-interceptor`](https://www.npmjs.com/package/node-request-interceptor) and [`@mswjs/interceptors`](https://www.npmjs.com/package/@mswjs/interceptors) to mock the backend requests, but they didn't work either due to not being detected or returning in invalid responses - [`nock`](https://www.npmjs.com/package/nock) worked smoothly out of the box.
- Collaborated on architectural design of social Recipe-based application & landing page.
- Assisted in implementation of Customizable Images feature of [Image Generalization Finder][igf].
- Researched solutions to obscure Terragrunt error messages.
- Repaired user-authentication in Cocktail-discovery MERN application.
- Setup Toon Boom Harmony development environment with VSCode.

## Day 002: January 3, 2023

|                                                              Codewar                                                               |                                                      LeetCode                                                       |                                                 Quotes                                                  |
| :--------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------: |
| [Remove the noise from the string](https://www.codewars.com/kata/reviews/5681d49e73153b608e000036/groups/56f92c42e4d45de6fd000044) | [Delete Columns to Make Sorted](https://leetcode.com/problems/delete-columns-to-make-sorted/submissions/870087609/) | [Joker](https://media-quotes.onrender.com/ejs/search?query=My+Life+Is+Nothing+But+A+Comedy&title=Joker) |

- Conquered a phantom serverless-NodeJS error about being unable to create some cache:
  - Discovered the issue by seeing lines related to cache creation once I turned the logging level up via the [`--loglevel=verbose`](https://docs.npmjs.com/cli/v8/using-npm/logging#loglevel) flag.
  - Running [`npm`](https://www.npmjs.com/) commands with the `--prefix` flag messed this up - but setting the `npm_config_cache` environment variable to `/tmp/` does the trick!
  - Led to the discovery that the barely-documented `--prefix` flag appears to be [planned for removal](https://github.com/npm/cli/issues/1368#issuecomment-1241076700).
- Created [Userscript](https://violentmonkey.github.io/) to add looping functionality to [Canva](https://www.canva.com/) videos for presentations:
  - ```javascript
    // Magic script to make Canva videos loop forever, execute when "Rewatch" button is visible at end of video
    document
      .evaluate("//p[contains(., 'Rewatch')]", document, null, XPathResult.ANY_TYPE, null)
      .iterateNext()
      .closest('div[role="button"]').style.display = 'none';
    document.querySelector('video').play();
    ```

## Day 003: January 4, 2023

|                                                               Codewar                                                                |                                               Quotes                                               |
| :----------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------: |
| [Euclidean distance in n dimensions](https://www.codewars.com/kata/reviews/5681d49e73153b608e000036/groups/56f92c42e4d45de6fd000044) | [Toy Story](https://media-quotes.onrender.com/ejs/search?query=falling+with+style&title=Toy+Story) |

- Took place in Mock Technical & Behavioral Interviews:
  - Led to the use of a [Circular Buffer / Ring Array](https://www.wikiwand.com/en/Circular_buffer) to add & compare items in constant time.

## Day 004: January 5, 2023

|                                                        Codewar                                                         |                                                    Quotes                                                    |
| :--------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------: |
| [More Zeros than Ones](https://www.codewars.com/kata/reviews/5d41ffef5f69ba0001ca7bd1/groups/63b71d9f67a144000151e9b3) | [Braveheart](https://media-quotes.onrender.com/ejs/search?query=Not+every+man+really+lives&title=Braveheart) |

- Assisted engineer with dynamically-valued [MUI Autocomplete](https://mui.com/material-ui/react-autocomplete/) controlled component that executed user-submitted code.
- Corrected manual setup instructions of OSS project.
- Explored [Admin.js](https://docs.adminjs.co/ui-customization/dashboard-customization) limitations and usability of Custom Components for a more visual & engaging experience.
- Developed the intersection of the Rerolling and Custom Image features of the [Image Generalization Finder][igf] MERN application.
