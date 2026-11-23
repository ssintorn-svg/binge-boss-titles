# binge-boss-titles

Runs the daily title-page job for [Binge Boss](https://bingeboss.tv). The job's code
and data live in a private repository; this repository only holds the schedule, so
the long, mostly idle runs (waiting on the language model's per-minute limits) use
GitHub's free minutes for public repositories.

The workflow checks out the private repository with a deploy key, writes and reviews
title texts, and pushes the result back. The daily content update there builds and
publishes the pages.
