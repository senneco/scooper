# scooper
it cleans up domain from lifecycle, special for you

## Manifest

1. Domain should not depends on Android application process lifecycle
1. One domain may depends on other domains
1. Domain should not depends on other domain's lifecycle

## How to realise these

1. Scooper save all domain's keys to the save state's `Bundle`
1. Each domain shouldn't receive direct link to other domain through constructor, setter, static provider e.t.c.
1. Scooper should provide domains to other domains
1. Each domain should have some initial method that allows Scooper to create that instance by keys from save state's `Bundle`

## How it can look like
