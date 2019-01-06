---
title: "What I learned about Ruby constants"
date: 2019-01-06T14:00:00-06:00
---

So today I got into the 3rd unit I did for [excercism](https://exercism.io/my/tracks), it was called Gigasecond. So I did struggle with a few things but I'm going to focus on the main problem I had, which was methods. My biggest struggle was and has been up until now figuring out what to do for a method. I talked to some people in the Ruby On Rails chat that I'm in and realized there are two seperate types of methods. Constant, and Instance, and with me being able to figure out the method, I looked more into constants. I realized that a constant can be used just by having a capital in something (or all caps) such as Gigasecond or GIGASECOND. ex: 

'''
class Gigasecond
  GIGASECOND = 10 ** 9
  def self.from(time)
    time + GIGASECOND
  end
end
'''

once I made GIGASECOND a constant (the constant being 10 ** 9 being 1,000,000,000) I realized I could use time + GIGASECOND(now being a constant) to figure out the time that the test was asking for. 
