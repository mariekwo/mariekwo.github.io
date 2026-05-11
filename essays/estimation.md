---
layout: essay
type: essay
title: "Guesstimation"
# All dates must be YYYY-MM-DD format!
date: 2026-05-10
published: true
labels:
  - Project Management
  - Time Managment
  - Estimation
---

<img width="200px" class="rounded float-start pe-4" src="../img/essay-img/crystalBall.png">

I've always had an uneasy relationship with time. Hours can fly by when I hyper fixate on something and minutes can creep slowly when I wish they would at least walk. For a recent school project we were directed to make time effort estimations on any work we needed to complete. I made my effort estimates by trying to relate the issue to previous issues. They were basically always off because I'm in my "I don't know what I don't know" stage. This phenomena is not exclusive to the project, I am terrible at estimating time in other parts of my life as well.Given that my estimates were so unreiable I'm not sure it was a worthwhile time expenditure.

To track the actual coding I used the reflog data on my local machine. It was hard to keep track of time without a dedicated timer because I did things other than coding in the time between commits. I tried using my phone's stopwatch but this didn't work well because I needed two different trackers-one for coding effort and one to keep track of non-coding effort. Since reflog data was the only time info I'm certain my time tracking is off. I used Claude Sonnet 4.6 to create a script that parsed the reflog data and use the creation, commit, and push times to estimate the time I spent on various issues. A prompt I used was "I want to use this reflog data to track time spent per issue. Should be able to adjust time between commits if it doesn't reflect actual time spent". This resulted in a somewhat usable application but I then had to direct it to account for branch creation times and to detect "detached head" work. This took a couple hours of back and forth but I now have this tool for use in the future, should I need it.

If I had to do this again I would use an app like WakaTime to log times for coding and non-coding effort. I'd also be interested in perhaps using AI to make estimates, but otherwise I'll just have to rely on experience!
