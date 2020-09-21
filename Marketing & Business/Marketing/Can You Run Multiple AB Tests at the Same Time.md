#ABtest #marketing 

Source: https://cxl.com/blog/can-you-run-multiple-ab-tests-at-the-same-time/

## What you should consider when running multiple simultaneous tests

Let’s first set the stage.

A user comes to your home page, making them part of test A. They then move on to the category page, and get to be a part of test B. Next, they go to the product page — which shows them test C. After, they add a product to cart — and are entered into test D. Finally, they completing checkout and test E is in full effect.

The user ends up buying something, and “conversion” is registered.

Questions:

- Did any of the variations in those tests influence each other, and thus skew the data? (Interactions)
- Which variation of which test gets the credit? Which of the tests really nudged the user into buying something? (Attribution)

### Why running multiple separate tests at the same time might be a bad idea:

Cross-pollination of users leads to **a much higher chance of a type 1 error** (false positive), as well as more daily and average variance, which means it is harder to have actionable results and even more likely you will get a false positive.  This is especially true for low volume sites, which are of course the ones most likely to want to run multiple tests at the same time.

The thing to realize is that there is no one way to be perfect with your testing.  What you are trying to maximize is your ability to maintain some data integrity and a valid population to answer questions, while also maximizing your ability to exploit your test results. It is very easy to dive off the deep end and convince yourself that cross-pollination or other things that can at times sound reasonable are so, but they violate very core disciplines in terms of testing.

Ideally you would not ever have multiple tests as they do add an increased likelihood of error, but if you are focusing all of your efforts on minimizing human error (with things like understanding variance, good test design and discipline, understanding distribution, minimizing bias, challenging assumptions, etc), then **there are times when it is an acceptable risk.**

The thing to remind yourself and others on though is that there is always a want to run faster, and the biggest problem with impacting the validity of your results is that bad results and good results look the same.  **You want to believe**, which means that the higher risk and the higher delta due to bad test design is hypnotic and draws in people.  It takes constant vigilance to avoid falling into that type of pitfall.

A testing tool vendor, Maximyser, advocates that running multiple tests at the same time results in low accuracy:

> It’s possible that the “interactions” between variants in the two tests are not equal to each other and uniformly spread out.

The argument is that there are cases where interaction effects between tests matter (often unnoticed), but it can have a major impact on your test conclusions. According to them, instead of simultaneous tests, it’d be better to combine the tests and run them as MVT.

As with most things in marketing and A/B testing, not everyone fully agrees:

There are merits to this approach, but they are mostly advocating a multivariate approach — which is fine but I’m not sure I’d categorically say simultaneous A/B tests on a site are always ripe with more risk than waiting (weeks) to introduce a new test, and ideally better design.

Matt Gershoff recommends you figure two things out before determining whether to run multiple separate tests at once:

- How likely are we in a situation in which there might be interactions between tests?
- How much overlap is there?

If only 1% of the users see both tests, then who cares. If it’s more like 99%, then ask yourself: “Do I really think there are going to be extreme interactions?” (Probably not.)

So in practice – unless you think there is going to be an issue, or it is a super important issue you are testing, then probably don’t sweat it.

### If the split between variations is always equal, doesn’t it balance itself out?

> Even if one test’s variation is having an impact on another test’s variations, the effect is proportional on all the variations in the latter test and therefore, the results should not be materially affected.

![[Pasted image 7.png]]

Some think this model is oversimplified, and the argument also implies that attribution is not important.

The question then is, do you really care about attribution?

You may or may not. If we want to know what really impacted user behavior, and which of the tests was responsible, then attribution does matter.

## Are you in the business of science, or in the business of making money?

The success of your testing program is comprised of the number of tests run (e.g. per year), the percentage of winning tests, and the average impact per successful experiment.

Now if you limit the number of tests you run for the sake of avoiding data pollution, you are also significantly reducing the velocity of your testing.

If your primary goal is to figure out the validity of a single test, to be confident in the attribution and the impact of the test, then you might want to avoid tests with overlapping traffic. But while you do that, you are not running all those tests that might give you a lift—and as a result potentially losing money.

Do you care more about the precision of the outcome, or making money?

Here’s what Lukas Vermeer thinks about running multiple tests at once on the same site:

No reason not to. Lots of reasons in favor of it.

Consider this: your competitor is probably also running at least one test on his site, and a) his test(s) can have a similar “noise effect” on your test(s) and b) the fact that the competition is not standing still means you need to run at least as many tests as he is just to keep up.

The world is full of noise. Stop worrying about it and start running as fast as you can to outpace the rest!

## Choose the right strategy

Ultimately, we want to run more tests, but we also want the results to be accurate. So what are the options that we have available to us? Matt Gershoff has done a [great job explaining the options here](http://conductrics.com/ab-testing-when-tests-collide-2/), related article also on the Maxymiser blog. I’m summarizing the 3 main strategies you should choose from:

1. **Run multiple separate tests**

Unless you suspect extreme interactions and a huge overlap between tests, this is going to be OK. You’re probably fine to do it, especially if what you test is not paradigm-changing stuff and there’s little overlap.

2. **Mutually exclusive tests**

Most testing tools give you the option to run mutually exclusive tests, so people wouldn’t be part of more than one test. The reason you’d want to do this is to eliminate noise or bias from your results. The possible downside is that it might be more complex to set this kind of tests up, and it will slow down your testing as you’ll need [an adequate sample size](https://cxl.com/stopping-ab-tests-how-many-conversions-do-i-need/) for each of these tests.

3. **Combine multiple tests into one, run as MVT**

If you suspect strong interaction between tests, it might be better to better to combine those tests together and run them as an MVT. This option makes sense if the tests you were going to run measure the same goal (e.g. purchase), they’re in the same flow (e.g. running tests on each of the multi-step checkout steps), and you planned to run them for the same duration.

MVT doesn’t make sense if Test A was going to be about an offer and Test B experimenting with the main navigation – low interaction.

## How to balance testing speed and accuracy of results?

Testing speed and accuracy of test results is a trade-off, and there is no single right answer here, although these three experts recommend similar approaches:

1. I try to balance the speed with the need for accuracy, especially on large changes. With my current program, if I am doing a large page design test on a major page, I will run that by itself with no other tests. If I am doing more mechanical discovery and exploitation tests, then I will try to time them to maximize total population. Most of the time I focus on having 1 “large” test with a larger percentage of my traffic and one “small” test which is usually something mechanical like copy testing or presentation tests.
2. There are two speeds to consider: the speed at which you crank out new experiments and the speed at which you run single experiments. I don’t believe you can ever be too fast on the former; try and test as many things as you can imagine or build. For the latter, you have to balance certainty of the result with the time spent on a single experiment; the slower you go, the more certainty you will have. How you balance these things depends on the experiment; or more specifically: what depends on the outcome. Are you testing a simple copy change or stock image or a new business model that might set company direction for the next five years? These two cases require different levels of certainty, and this different speeds.
3. If you have a test that is REALLY important, then you make sure you are more careful. It is all about taking educated risk. So unless there is reason to do otherwise, one should just do what is simple, but we should be aware of all the possibilities even if the more complex cases are fairly rare. This way we can at least be in a position to evaluate if we are ever in one of the more complex situations. Start with speed/quantity (especially if there’s minimal overlap), and then pick your battles for the more complex problems.

## Conclusion
Like with most things business and marketing, there’s no easy answer.

In many cases, running multiple simultaneous tests makes sense. Unless you’re testing really important stuff (e.g. something that impacts your business model, future of the company), the benefits of testing volume will most likely outweigh the noise in your data and occasional false positives.

If based on your assessment there’s a high risk of interaction between multiple tests, reduce the number of simultaneous tests and/or let the tests run longer for improved accuracy.



