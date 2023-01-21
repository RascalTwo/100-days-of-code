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

## Day 005: January 6, 2023

[vum]: https://github.com/RascalTwo/VideoUserMarkers

|                                                                  Quotes                                                                  |
| :--------------------------------------------------------------------------------------------------------------------------------------: |
| [2001: A Space Odyssey](https://media-quotes.onrender.com/ejs/search?query=I%27m+afraid+I+can%27t+do+that&title=2001%3A+A+Space+Odyssey) |

- Released the MVP of [Video User Markers][vum] website.
- Recovered nearly-lost changes to a `git` repository - don't forget that [`git reflog`](https://git-scm.com/docs/git-reflog) is your friend!

## Day 006: January 7, 2023

|                                                    Quotes                                                    |
| :----------------------------------------------------------------------------------------------------------: |
| [Top Gun: Maverick](https://media-quotes.onrender.com/ejs/search?query=Extinction&title=Top+Gun%3A+Maverick) |

- Released [Heroku Migrations](https://rascaltwo.com/blog/heroku-migrations) blog post.

## Day 007: January 8, 2023

|                                                                      Codewar                                                                      |                                        Quotes                                        |
| :-----------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------: |
| [Help Grinch steal Christmas from JS programmers](https://www.codewars.com/kata/reviews/633872d87301f100011c0c99/groups/63a6531b48f9d30001946002) | [Die Hard](https://media-quotes.onrender.com/ejs/search?query=Yippee&title=Die+Hard) |

- Implemented authentication-related messaging for OAuth-based MERN application.
- Wrote code to implement simplified routing in mockup of a React application.

## Day 008: January 9, 2023

[cyclic]: https://www.cyclic.sh/

|                                                       Codewar                                                        |                                                    Quotes                                                     |
| :------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------: |
| [Frequency sequence](https://www.codewars.com/kata/reviews/5862b4af877993caae00103d/groups/63bc6f1d3701370001baa564) | [The Sixth Sense](https://media-quotes.onrender.com/ejs/search?query=I+see+dead+people&title=The+Sixth+Sense) |

- Assisted engineer setting up production-ready deployment of a Monorepo MERN application to [Cyclic.sh][cyclic].
- Setup production deployment of OpenAPI-based MERN application to [Cyclic.sh][cyclic].
- Researched unexpected breaking-changes to the [EDAMAN Food API](https://developer.edamam.com/food-database-api-docs):
  - Passing a brand to `ingr` was previously handled, but now returns an `java.lang.IllegalArgumentException` error.
  - Must now be passed under the `brand` parameter.
- Collaborated on the design of a social Recipe MERN application.

## Day 009: January 10, 2023

|                                                      Codewar                                                       |                                                  Quotes                                                   |
| :----------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------: |
| [Doubleton number](https://www.codewars.com/kata/reviews/604287c26f2b2b00019ca1e4/groups/63bdb695ae550f0001cc5353) | [The Truman Show](https://media-quotes.onrender.com/ejs/search?query=Say+Something&title=The+Truman+Show) |

- Customized GatsbyJS application to support more dynamic data.
- Resolved an issue with successful & failure models not appearing on a React-based Contact Form.
- Hooked up HTML5 Canvas output to a file input.
- Implemented Embedability in [Video User Markers][vum].

## Day 010: January 11, 2023

|                                                       Codewar                                                        |                                                                     LeetCode                                                                      |                                                          Quotes                                                          |
| :------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------: |
| [Make a square box!](https://www.codewars.com/kata/reviews/58796860c0f4cbb6740005ba/groups/63beec305ee66e00019d00cf) | [Minimum Time to Collect All Apples in a Tree](https://leetcode.com/problems/minimum-time-to-collect-all-apples-in-a-tree/submissions/876258013/) | [The Wolf of Wall Street](https://media-quotes.onrender.com/ejs/search?query=nobody+knows&title=The+Wolf+of+Wall+Street) |

- Refactored React-Query-based protected routes.
- Improve usability of [Video User Markers][vum]:
  - Made the parsing of raw markers more robust.
  - Implemented Markdown rendering of descriptions.

## Day 011: January 12, 2023

|                                                      Codewar                                                      |                                                                            LeetCode                                                                             |                                                    Quotes                                                     |
| :---------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------: |
| [Run your String](https://www.codewars.com/kata/reviews/54cb616e4fdf30334a000296/groups/54cf832b6b85dc5e63000df8) | [Number of Nodes in the Sub-Tree With the Same Label](https://leetcode.com/problems/number-of-nodes-in-the-sub-tree-with-the-same-label/submissions/876724685/) | [Shutter Island](https://media-quotes.onrender.com/ejs/search?query=You+Came+Here+Alone&title=Shutter+Island) |

- Guided college through getting their pet adoption application production ready & deployed.
- Made [Video User Markers][vum] more appealing to third parties:
  - Added URL-powered data loading and dedicated `<iframe>`-able pages.
  - Ability to clone and fork existing collections, with collection creation form directly linkable.
  - Implemented rich embed support, both generically and for Discord.

## Day 012: January 13, 2023

|                                                      Codewar                                                      |                                                                    Quotes                                                                     |
| :---------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------: |
| [Assemble String](https://www.codewars.com/kata/reviews/6210fc41cf0a220001821f42/groups/63c1836e4dc4530001f427e2) | [Monty Python and the Holy Grail](https://media-quotes.onrender.com/ejs/search?query=Tis+but+a+scratch&title=Monty+Python+and+the+Holy+Grail) |

- Implemented importing of initial YouTube chapters into Markers to [Video User Markers][vum].
- Additionally added customizable sorting on all [Video User Markers][vum] listing-pages.

## Day 013: January 14, 2023

[render]: https://render.com/

|                                                  Quotes                                                  |
| :------------------------------------------------------------------------------------------------------: |
| [Finding Nemo](https://media-quotes.onrender.com/ejs/search?query=Just+keep+swimming&title=Finding+Nemo) |

- Dockerized & deployed a Java Spring Boot project to [Render][render].
- Released [Getting Production Ready](https://rascaltwo.com/blog/getting-production-ready) blog post.

## Day 014: January 15, 2023

|                                                         Codewar                                                         |                                                  Quotes                                                  |
| :---------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------: |
| [Address Book by State](https://www.codewars.com/kata/reviews/5a7c604b5d173c9d40000a6a/groups/63c468563841230001d86554) | [Finding Dory](https://media-quotes.onrender.com/ejs/search?query=just+keep+swimming&title=Finding+Dory) |

- Created MVP for serverless NPM CWD-changing errors.

## Day 015: January 16, 2023

[mq-api]: https://github.com/RascalTwo/Quotes

|                                                       Codewar                                                       |                                        Leetcode                                         |                                                  Quotes                                                   |
| :-----------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------: |
| [Alternating Loops](https://www.codewars.com/kata/reviews/55e52b5e910dcb94300000b1/groups/63c573840b23c40001a1a772) | [Insert Interval](https://leetcode.com/problems/insert-interval/submissions/879304840/) | [Gone with the Wind](https://media-quotes.onrender.com/ejs/search?query=frankly&title=Gone+with+the+Wind) |

- Implemented Dark theme within [Video User Markers][vum].
- Added media-dropping script to [Media Quotes][mq-api].

## Day 016: January 17, 2023

|                                                      Codewar                                                      |                                                           LeetCode                                                            |                                               Quotes                                                |
| :---------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------: |
| [Combinator Flip](https://www.codewars.com/kata/reviews/541b66f0dc648f86910001e3/groups/55c7eb6442b45991230000ff) | [Flip String to Monotone Increasing](https://leetcode.com/problems/flip-string-to-monotone-increasing/submissions/880000019/) | [Inside Out](https://media-quotes.onrender.com/ejs/search?query=inside+their+head&title=Inside+Out) |

- Added XPI-publishing script & Landing Page to [Video User Markers][vum].
- Implemented authentication in a social Recipe-based MERN application.

## Day 017: January 18, 2023

[pws]: https://github.com/RascalTwo/PairwiseSorter

|                                                   Codewar                                                    |                                                      LeetCode                                                       |                                                    Quotes                                                    |
| :----------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------: |
| [Free Pizza](https://www.codewars.com/kata/reviews/5962e9f9c409116f9d001677/groups/63c8075c39c9410001d191e3) | [Maximum Sum Circular Subarray](https://leetcode.com/problems/maximum-sum-circular-subarray/submissions/880605435/) | [Catch Me If You Can](https://media-quotes.onrender.com/ejs/search?query=catch+me&title=Catch+Me+If+You+Can) |

- Various [Pairwise Sorter][pws] improvements:
  - Implemented sorting-persistance when deleting items.
  - Resolved edge-case issue when deleting items.
- Resolved rendering issue with [Media Quotes API][mq-api].
