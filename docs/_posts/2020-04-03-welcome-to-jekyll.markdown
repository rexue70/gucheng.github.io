---
layout: post
title:  "Leetcode 1. Two Sum"
date:   2020-04-03 19:33:31 -0700
categories: jekyll update
---
This is a testing page for 古城, welcome!

{% highlight java %}
    public int[] twoSum(int[] nums, int target) {
        Map<Integer, Integer> map = new HashMap<>();
        for (int i = 0; i < nums.length; i++) {
            int diff = target - nums[i];
            if (map.containsKey(diff)) return new int[]{map.get(diff), i};
            map.put(nums[i], i);
        }
        return null;
    }
{% endhighlight %}

