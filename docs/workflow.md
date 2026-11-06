# Workflows

## Scheduling and execution rules
- Workflow A: Monday, Wednesday, Friday at 10:00 AM.
- Workflow B: Monday at 9:00 AM.
- Tuesday, Thursday, and weekends are publishing days off.
- Never publish outside the Mon/Wed/Fri 10:00 AM windows.
- Schedules change only with owner authorization.
- Time zone: unverified.

## Workflow A: Content Briefing & Publishing
1. **Trend research:** search the web for trending topics in AI product design, AI tools, and AI careers.
2. **History retrieval:** fetch the last 15 `ContentPost` records; avoid topics from the last 10 posts.
3. **Content generation:** one story-first post in first-person voice, built on a real project, build, or experience. Structure: hook, personal story, one practical lesson, one simple conversational question.
4. **Image generation:** create a relevant AI image.
5. **Publishing:** publish the post with the image; save the LinkedIn post URN and publishing status in `ContentPost`; set status to `posted` on success.
6. **Comment engagement:** check the last three posts for unanswered comments; generate and publish replies in the owner's conversational voice, where the implemented workflow permits.
7. **Notification:** send the owner the hook, the reasoning behind the content, and the LinkedIn link.

### Topic deduplication
Compare candidate topics with the last 10 posts (from the 15 retrieved). A candidate that overlaps is discarded and another is chosen. The exact similarity method is unverified.

### Factual integrity
The post must come from real projects or experiences supplied by the owner or recorded in project data. If no verifiable story is available, the workflow should not fabricate one (handling is unverified; see error handling).

## Workflow B: Weekly Engagement Report
1. Retrieve engagement data for every post published in the previous two weeks.
2. Collect available likes and comments.
3. Identify the top-performing post.
4. Analyse content themes and engagement patterns.
5. Examine timing patterns.
6. Recommend topics and approaches to double down on.
7. Generate and send the weekly report.

### Methodology notes
Analysis is limited to metrics the LinkedIn integration exposes. With only a few posts in a two-week window, patterns are indicative, not statistically conclusive. Because posts publish at a fixed time, timing analysis is limited to day-of-week effects.

## Automation level
| Operation | Level |
|---|---|
| Scheduled triggers | Automated |
| Research, generation, image, publishing | Automated |
| Saving URN and status | Automated |
| Comment replies | Automated where the implemented workflow permits; extent unverified |
| Owner notification | Automated |
| Weekly report | Automated |
| Schedule changes, credential renewal, supplying real project stories | Manual |
