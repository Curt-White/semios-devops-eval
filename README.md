# semios-devops-eval

Total Time Taken: ~1.75 hours

URL: https://curtscrazyclocks.surge.sh/

Important Points:
* I do not have quite as detailed notes as Ken regarding exact times since the time I spent on it was broken up by meetings throughout the day.
* This is coming from someone who has never used github actions before, I am certain this would be quicker for someone who has setup these kind of systems in the past (they might even find it quite easy)
* I feel that someone with proper github actions and repo config experience could manage this in less than an hour

* This design uses only two separate Github actions yml files. One of them is for the deploy and the other is for the testing.
* Extremely helpful to have the actions addon for surge (prevents the need for npm or any other shell scripting and probably cuts down the time a bunch)

* The revised assessment fixed the majority of my initial confusions

* Quite straight forward and think it is much better without having a fork anyways!

Point of Confusion:
* Not really that confusing as it seems like there is a fair amount of freedom. But I was not completely sure if you wanted the surge site deployed in the PR after the tests passed or after there was a successful merge into master. Is this up to the person to decide. This is the related deliverable: "One PR clearly labelled in which the test suite ispassing, and a correspondingsurge.sh site is deployed with the latest git commithash embedded in theindex.html file". In the end it made more sense to me to deploy after a merge with master then to have the deploy action in the pull request before the merge.
