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

## Day 018: January 19, 2023

|                                                       Codewar                                                       |                                                     LeetCode                                                      |                                                       Quotes                                                        |
| :-----------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------: |
| [Trimming a string](https://www.codewars.com/kata/reviews/563fb348f47611dae800003e/groups/63c9ba2bb7f1970001ef5fce) | [Subarray Sums Divisible by K](https://leetcode.com/problems/subarray-sums-divisible-by-k/submissions/881474264/) | [James and the Giant Peach](https://media-quotes.onrender.com/ejs/?query=top+of+it&title=James+and+the+Giant+Peach) |

- Setup CI/CD for a Next.js project.
- Optimized deployment of scheduling application, additionally assisted implementing welcoming of new users.
- Implemented welcoming of new users

## Day 019: January 20, 2023

|                                                                      Codewar                                                                       |                                                    LeetCode                                                     |                                                    Quotes                                                    |
| :------------------------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------: |
| [How fast can the burglar steal all the diamonds?](https://www.codewars.com/kata/reviews/63a1a8f8ba5c59000119c4d0/groups/63cadf324907d80001c27fd1) | [Non-decreasing Subsequences](https://leetcode.com/problems/non-decreasing-subsequences/submissions/881987038/) | [Alita: Battle Angel](https://media-quotes.onrender.com/?title=Alita%3A+Battle+Angel&query=presence+of+evil) |

- Implemented Lazy-Loading of custom items in [Pairwise Sorter][pws], accompanied by explicit confirmation dialogs before deletion & resetting.
- Participated in a Technical Assessment.
- Assisted college in setup of a TypeScript project.

## Day 020: January 21, 2023

|                                                                  Codewar                                                                  |                                            LeetCode                                             |                                          Quotes                                          |
| :---------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------: |
| [Find the Nexus of the Codewars Universe](https://www.codewars.com/kata/reviews/57bfc1c12328dfb7bf000008/groups/63cc1bfacb15720001439323) | [Restore IP Address](https://leetcode.com/problems/restore-ip-addresses/submissions/882563698/) | [Aladdin](https://media-quotes.onrender.com/?title=Aladdin&query=Genie%2C+you%27re+free) |

- Add search functionality to [Pairwise Sorter][pws], additionally normalized rendering of items.
- Participated in a Technical Assessment.
- Fixed initial collection parsing issue in [Video User Markers][vum].

## Day 021: January 22, 2023

|                                                   Codewar                                                   |                                                LeetCode                                                 |                                        Quotes                                         |
| :---------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------: |
| [Smart Sum](https://www.codewars.com/kata/reviews/58312013b812b8016d000096/groups/63cd8868568d480001d96e6d) | [Palindrome Partitioning](https://leetcode.com/problems/palindrome-partitioning/submissions/883259556/) | [The Iron Giant](https://media-quotes.onrender.com/?query=I+fix&title=The+Iron+Giant) |

- Implement client-side dynamic searching in [Pairwise Sorter][pws] with highlighting, additionally the ability for users to see completed items sorted.
- Various [Video User Marker][vum] improvements:
  - Added Quickstart page.
  - Stabilize sorting.
  - Improve extension stability & resilience.
  - Automatically pause videos during the creation of markers.
  - Document API for third-party usage.

## Day 022: January 23, 2023

|                                                     Codewar                                                      |                                            LeetCode                                             |                                  Quotes                                  |
| :--------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------: |
| [Perfect Square](https://www.codewars.com/kata/reviews/584eb705e07fd70844000a9e/groups/63ceb7310592720001a4e9ef) | [Find the Town Judge](https://leetcode.com/problems/find-the-town-judge/submissions/883811196/) | [Se7en](https://media-quotes.onrender.com/?query=in+the+box&title=Se7en) |

- Setup CRX generation of [Video User Markers][vum].
- Resolve modal styling & user directing issues in event-scheduling application.

## Day 023: January 24, 2023

|                                                                     Codewar                                                                     |                                           LeetCode                                            |                                            Quotes                                            |
| :---------------------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------: |
| [RoboScript #1 - Implement Syntax Highlighting](https://www.codewars.com/kata/reviews/5870a9f4548efaf35e00111f/groups/63cff93279a532000181e523) | [Snakes and Ladders](https://leetcode.com/problems/snakes-and-ladders/submissions/884438725/) | [The WIcker Man](https://media-quotes.onrender.com/?title=The+Wicker+Man&query=not+the+bees) |

- Converted EJS to JSX in [Video User Markers][vum].

## Day 024: January 25, 2023

|                                                    Quotes                                                    |
| :----------------------------------------------------------------------------------------------------------: |
| [How to Train Your Dragon](https://media-quotes.onrender.com/?query=gestured&title=How+to+Train+Your+Dragon) |

- Started backend-deployment simulator.

## Day 025: January 26, 2023

|                                                                 Codewar                                                                  |                                                            Quotes                                                             |
| :--------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------: |
| [Sort Strings by Most Contiguous Vowels](https://www.codewars.com/kata/reviews/5d305f3f5228cc0001e4967b/groups/63d2e2975e25f20001f4c533) | [How to Train Your Dragon 2](https://media-quotes.onrender.com/?query=control+of+bad+people&title=How+to+Train+Your+Dragon+2) |

- Participated in [Together][together] demo to [Cyclic.sh][cyclic].
- Optimized custom-item-loading in [Pairwise Sorter][pws].

## Day 026: January 27, 2023

|                                                              Codewar                                                               |                                                                             Quotes                                                                             |
| :--------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| [Simple Fun #51: Election Winners](https://www.codewars.com/kata/reviews/58881c042e973aab72001f51/groups/63d4166763ffb400010f71b9) | [How to Train Your Dragon: The Hidden World](https://media-quotes.onrender.com/?query=with+love+comes+loss&title=How+to+Train+Your+Dragon%3A+The+Hidden+World) |

- Add Renaming & Deletion actions to comparison view, and conditional custom item rendering based on current view to [Pairwise Sorter][pws].

## Day 027: January 28, 2023

|                                                         Codewar                                                          |                                       Quotes                                        |
| :----------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------: |
| [Remove the parentheses](https://www.codewars.com/kata/reviews/5f8716db6ddaa30001d6378a/groups/63d57bbbddf4f50001a252c0) | [Astro Boy](https://media-quotes.onrender.com/?query=old+fashioned&title=Astro+Boy) |

- Add raw Video/Audio support to [Video User Markers][vum].

## Day 028: January 29, 2023

|                                                                   Codewar                                                                   |                                                Quotes                                                |
| :-----------------------------------------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------: |
| [The unknown but known variables: Addition](https://www.codewars.com/kata/reviews/5719325c4c82d0a01f00006c/groups/63d6b8700aa2010001462e2b) | [Groundhog Day](https://media-quotes.onrender.com/?query=is+it+snowing+in+space&title=Groundhog+Day) |

- Got Production-Deployment simulator to a publicly usable state.

## Day 029: January 30, 2023

|                                                               Codewar                                                               |                                               Leetcode                                                |                                 Quotes                                  |
| :---------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------: |
| [Thinkful - Object Drills: Vectors](https://www.codewars.com/kata/reviews/5a1c5aaa3d6f011119001da7/groups/5f561ad415fbdc000188fd37) | [N-th Tribonacci Number](https://leetcode.com/problems/n-th-tribonacci-number/submissions/888367083/) | [Jaws](https://media-quotes.onrender.com/?query=bigger+boat&title=Jaws) |

- Completed a Frontend technical assessment

## Day 030: January 31, 2023

|                                                      Codewar                                                      |                                             Quotes                                              |
| :---------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------: |
| [Cyclops numbers](https://www.codewars.com/kata/reviews/5e83db0fee30ee0001df84dc/groups/63d96d4b0a865a00016c9810) | [Ratatouille](https://media-quotes.onrender.com/?query=fearless+can+be+great&title=Ratatouille) |

- Populate deployment simulator with various defaults
- Assisted debugging and proper association of Sequelize entities.

## Day 031: February 01, 2023

|                                                          Codewar                                                          |                                                           LeetCode                                                            |                                                         Quotes                                                         |
| :-----------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------------: |
| [1's, 0's, and wildcards](https://www.codewars.com/kata/reviews/588f504dc67019652e0012b0/groups/63dae9e5fd54250001e515f3) | [Greatest Common Divisor of Strings](https://leetcode.com/problems/greatest-common-divisor-of-strings/submissions/889711382/) | [Mr. & Mrs. Smitch](https://media-quotes.onrender.com/?query=name+and+social+security+number&title=Mr.+%26+Mrs.+Smith) |

- Improve usage of fully-sorted lists in [Pairwise Sorter][pws].

## Day 032: February 02, 2023

|                                                                      Codewar                                                                       |                                                      LeetCode                                                       |                                                     Quotes                                                     |
| :------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------: |
| [Unknown amount of duplicates. One missing number](https://www.codewars.com/kata/reviews/5b8cea4a6645f1b991000342/groups/63dbb6b5d919fb00012bfd7c) | [Verifying an Alien Dictionary](https://leetcode.com/problems/verifying-an-alien-dictionary/submissions/890060500/) | [Treasure Planet](https://media-quotes.onrender.com/?query=help+people+with+a+doctorate&title=Treasure+Planet) |

- Add cloning to [Pairwise Sorter][pws] lists and improved searching responsiveness.
- Assisted in getting [100Devs-MERN-Starter-Kit](https://github.com/isaaclee12/100Devs-MERN-Starter-Kit) production-ready.
- Participated in JavaScript technical assessment.

## Day 033: February 03, 2023

|                                                      Codewar                                                      |                                          LeetCode                                           |                                        Quotes                                        |
| :---------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------: |
| [Nothing special](https://www.codewars.com/kata/reviews/5871f3a8c7e00b129400025c/groups/5871f3a8c7e00b1294000260) | [Zigzag Conversion](https://leetcode.com/problems/zigzag-conversion/submissions/890725985/) | [Logan](https://media-quotes.onrender.com/?query=Someone+HAS+come+along&title=Logan) |

- Fixed unresponsive landing page layouts.
- Created automated post-responding Playwright script.
- Assisted teammate with [Together][together] issue and malformed git repository.

## Day 034: February 04, 2023

|                                                  Codewar                                                  |                                              LeetCode                                               |                                              Quotes                                              |
| :-------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------: |
| [Ziiiiip](https://www.codewars.com/kata/reviews/5298ad7cd0f550269500051e/groups/63deda963c1f520001ecf269) | [Permutation in String](https://leetcode.com/problems/permutation-in-string/submissions/891616146/) | [The Lego Movie](https://media-quotes.onrender.com/?query=total+perfection&title=The+Lego+Movie) |

- Participated in Takehome Web Development assessment.

## Day 035: February 05, 2023

|                                                       Codewar                                                       |                                          LeetCode                                           |                                         Quotes                                         |
| :-----------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------: |
| [What comes after?](https://www.codewars.com/kata/reviews/590f7c32415127c7530003a2/groups/63e04f7f5431af0001416944) | [Shuffle the Array](https://leetcode.com/problems/shuffle-the-array/submissions/892327041/) | [That '70s Show](https://media-quotes.onrender.com/?query=foot&title=That+%2770s+Show) |

- Setup song-processing pipeline.

## Day 036: February 06, 2023

- Created Cypress E2E tests for [Together][together].

## Day 037: February 07, 2023

- Finished Cypress E2E tests [Together][together].

## Day 038: February 08, 2023

|                                                               Codewar                                                               |                                          Quotes                                           |
| :---------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------: |
| [Parse a linked list from a string](https://www.codewars.com/kata/reviews/582ff15655f28efa32000046/groups/63e3ccdecff68500012368bf) | [Ford v Ferrari](https://media-quotes.onrender.com/?query=go+to+war&title=Ford+v+Ferrari) |

- Managed user & organization OneDrive permissions.
- Debugged cross-platform incompatibility issues with production-deployment.
- Participated in Technical Assessment.

## Day 039: February 09, 2023

[fott]: https://github.com/JoeSangine/image-generalization-finder

|                                                                Codewar                                                                |                                         LeetCode                                          |                                      Quotes                                      |
| :-----------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------: |
| [Conway's Look and Say - Generalized](https://www.codewars.com/kata/reviews/530045e3c7c0f4d3420001b2/groups/63e580a4bfb4790001458292) | [Naming a Company](https://leetcode.com/problems/naming-a-company/submissions/895018679/) | [Alien](https://media-quotes.onrender.com/?query=answer+is+negative&title=Alien) |

- Initialized [Furred of the Third][fott].
- Assisted in repair of [Image Generalization Finder][igf].
- Collaborated in the token-level customization of a VSCode theme.

## Day 040: February 10, 2023

|                                                        Codewar                                                         |                                                        Quotes                                                         |
| :--------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------: |
| [Is there an Odd Bit?](https://www.codewars.com/kata/reviews/5ea5c0ab1be43d000155c119/groups/63e67ed0cd329c0001a0eb3a) | [Django Unchained](https://media-quotes.onrender.com/?query=curious+what+makes+you+so+curious&title=Django+Unchained) |

## Day 041: February 12, 2023

- Assisted in setup of CI & CD for [Together][together].
- Onboarded new developer into Blazor project.

## Day 042: February 13, 2023

|                                                         Codewar                                                          |                                                               LeetCode                                                                |                                      Quotes                                      |
| :----------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------: |
| [A Promise is a Promise](https://www.codewars.com/kata/reviews/5b61e20696bcb1f8750012df/groups/61da8dfe70fffc0001dd7906) | [Count Odd Numbers in an Interval Range](https://leetcode.com/problems/count-odd-numbers-in-an-interval-range/submissions/897209845/) | [The Shining](https://media-quotes.onrender.com/?query=Johnny&title=The+Shining) |

- Guided new developer through Cypress testing methodologies.

