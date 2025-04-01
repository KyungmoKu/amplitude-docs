---
id: 61370d33-6a3c-41a3-ba21-85ccaf8e861b
blueprint: event-segmentation
title: 'Build an event segmentation analysis'
source: 'https://help.amplitude.com/hc/en-us/articles/360052274852-Build-an-event-segmentation-analysis'
this_article_will_help_you:
  - 'Use events and properties to create an Event Segmentation analysis'
updated_by: 0c3a318b-936a-4cbd-8fdf-771a90c297f0
updated_at: 1743537618
landing: true
landing_blurb: 'Use events and properties to create an Event Segmentation analysis'
academy_course:
  - 49a7ec41-cae7-4f77-8f8f-e0a5101ce1df
---
For most users, Event Segmentation is the foundational Amplitude chart. It shows what your users are doing in your product. With the **Event Segmentation chart**, you can build analyses that:

* Measure the top events performed over a selected time period
* Analyze how often users trigger events
* Determine the count of unique users triggering events in your product
* Clarify which users tend to trigger certain events

Like most Amplitude charts, Event Segmentation charts combine events and event properties with user segments. These can be simple—like, for example, counting the number of users firing a specific event—or they can be intricate formulas of events. 

This article describes the steps required to build a segmentation analysis in Amplitude.

### Feature availability

This feature is available to users on **all Amplitude plans**. See the [pricing page](https://amplitude.com/pricing) for more details.

## Before you begin

If you haven’t already read up on the basics of [building charts in Amplitude](/docs/analytics/charts/build-charts-add-events), you should do so before proceeding.

See this article to read about [selecting the best measurement for your Event Segmentation chart](/docs/analytics/charts/event-segmentation/event-segmentation-choose-measurement).

## Set up an event segmentation analysis

An event segmentation analysis shows what different groups of users are doing in your product. You’ll need to tell Amplitude what events you're interested in, and which users it should include in the analysis.

{{partial:admonition type='note'}}
You can include both active and inactive events in your segmentation analyses, but most customers find their Amplitude charts are more insightful when they focus on active events.
{{/partial:admonition}}

To build an Event Segmentation chart, follow these steps:

1. In the Events Module, select the starting event or metric. You can choose a specific event that's instrumented in Amplitude, or you can tell Amplitude to consider any event as the starting event for this analysis, by selecting *Any Event* from the list of available events.  
  
    You can also [create an in-line custom event](/docs/analytics/charts/event-segmentation/event-segmentation-in-line-events) or [create a new metric](/docs/analytics/charts/data-tables/data-tables-create-metric) at this point, if you need to.

2. If desired, add properties to your starting event by clicking on *+ Filter by*, selecting the property name, and specifying the property value you’re interested in.

    {{partial:admonition type='note'}}
    The list of property values includes those ingested into your project during the last 30 days.
    {{/partial:admonition}}
   
3. Next, select another event to include, if desired. You can choose up to ten, and you can add properties to these events as well.

4. In the Measured As Module, specify how you'd like to measure your results. Unique users and event totals are the most commonly used, but you have several other options to select from.

5. In the Segmentation Module, identify the user segment you want to include in this analysis. You can import a already saved segment by clicking *Saved* and selecting the one you want from the list. Otherwise, Amplitude begins from the assumption that your analysis targets all users.  
  
{{partial:admonition type='note'}}
The user segment you select applies to all selected events.
{{/partial:admonition}}

1. If you don't want to import an already saved user segment, you can start building your own by adding properties. To do so, click *+ Filter by*, choose the property you want to include, and specify the property value you’re interested in.

2. You can narrow your focus even further by telling Amplitude you only want to include users who have already performed certain actions. To do so, click *+ Performed*, then choose the event you’re interested in.

3. If desired, add another user segment by clicking *+ Add Segment*, and repeating steps 6 and 7.

{{partial:admonition type='note'}}
You can break out your starting event by user properties by clicking *Group segment by* in the Segmentation Module, if desired. For example, if you wanted to group users by the cities they were in when they triggered the starting event, you would select *City* from the property list. Amplitude breaks out the segmentation analysis on a city-by-city basis.
{{/partial:admonition}}

In the chart area, you should now see your Event Segmentation chart, along with a tabular view of your results. 

[Read this article to find out how to choose the best measurement for your Event Segmentation chart](/docs/analytics/charts/event-segmentation/event-segmentation-choose-measurement).

To learn how to [interpret your event segmentation analysis](/docs/analytics/charts/event-segmentation/event-segmentation-interpret-1), check out this Help Center article.