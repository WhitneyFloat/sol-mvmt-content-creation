
name: Sol Mvmt Social Media Best Practices description: Guidelines for generating contextual captions and posting content to Instagram for Sol Mvmt brand
Sol Mvmt Social Media Best Practices
When tasked with creating social media posts for Sol Mvmt, the Agent must adhere to these best practices to ensure high-quality and on-brand content.

1. Contextual Caption Generation
You must never post a generic, default caption. How you generate the caption depends on the media type (image vs. video).
For Images
Call view_file on the image path to see the visual content
The system will provide an inline display of the visual elements
Analyze the aesthetics, tone, setting, and subjects of the image
Write a high-quality, engaging caption tailored to the specific content, including:
Relevant emojis (1-2 maximum, used sparingly)
Appropriate hashtags from the brand strategy
A clear call-to-action when relevant (e.g., "Link in bio," "Join us Sunday")
For Videos
You CANNOT visually analyze video files. The view_file tool does not support .mp4 and similar video formats.
Instead, follow this fallback flow to gather enough context for a great caption:
Check for a brand file first: Look for any *_BRAND.md file in the references/ folder. If one exists, read it and use the brand voice, tone, and audience to craft the caption.
If no brand file exists, ask the user: Prompt them with something like: "I can't peek inside videos directly — could you give me a quick description of what's in this video? Or point me to a brand guidelines file? That way I can write a caption that really nails the vibe." 
Use whatever context is available: The filename, the user's request, any accompanying notes, and the target platforms all help. Combine these into a contextually rich caption.
Write the caption using the Sol Mvmt voice:
Reflective and contemplative
Warm and inviting
Connected to deeper meaning
Include 1-2 emojis maximum
Include relevant hashtags
Clear structure (opening, body, close)

2. Getting Media Into Blotato
A decision tree for how to get images/videos to Blotato:
Option A: URL Passthrough (Preferred)
If the user provides a direct URL to the media file:
Use that URL directly in the Blotato post
No need to download or re-upload
Fastest and most efficient method
Option B: File Upload
If the media is a local file:
Use kite.ai upload functionality
Get the returned URL
Pass that URL to Blotato
Option C: Base64 Upload (Fallback)
If neither URL nor file upload works:
Encode the file as base64
Include in the Blotato API call
Only use when other methods fail
Best Practice: Always try URL passthrough first, then file upload, then base64 as last resort.

3. Platform-Specific Requirements
Quick reference for what each platform needs:
Instagram
Image Requirements:
Aspect ratios: 1:1 (square), 4:5 (portrait), 1.91:1 (landscape)
Recommended: 1080x1080px (square) or 1080x1350px (portrait)
Format: JPG or PNG
Video Requirements:
Reels: 9:16 (vertical), 1080x1920px
Feed: 1:1 or 4:5
Length: Up to 90 seconds (Reels), 60 seconds (Feed)
Format: MP4
Caption:
Max 2,200 characters
First 125 characters are preview (hook here!)
Hashtags: 8-15 recommended (max 30)
Location tags when relevant (San Tan Valley, Arizona)
Best Practices:
Post during optimal times: 7-9 AM, 12-1 PM, 7-9 PM Arizona time
Use 1-2 emojis maximum
Include call-to-action in last line
Tag @sol_mvmt_collective in collaborations
TikTok
Video Requirements:
Aspect ratio: 9:16 (vertical)
Resolution: 1080x1920px
Length: 15-60 seconds optimal
Format: MP4
Caption:
Max 2,200 characters (but shorter is better)
Hook in first 3 seconds of video AND caption
Hashtags: 3-5 focused tags
Trend participation only if on-brand
YouTube
Video Requirements:
Aspect ratio: 16:9 (horizontal) or 9:16 (Shorts)
Resolution: 1080p minimum
Format: MP4
Title & Description:
Title: 60 characters, front-load keywords
Description: Detailed, include timestamps if relevant
Tags: 5-10 relevant keywords

4. Timezone Conversion
Convert your local time to UTC for scheduling.
Sol Mvmt Location: Arizona (MST - No DST)
Arizona does NOT observe Daylight Saving Time
UTC offset: UTC-7 (year-round)
Conversion Examples:
7:00 AM Arizona → 14:00 UTC (2:00 PM UTC)
12:00 PM Arizona → 19:00 UTC (7:00 PM UTC)
7:00 PM Arizona → 02:00 UTC next day (2:00 AM UTC)
Formula: Arizona Time + 7 hours = UTC Time
Optimal Posting Times (UTC):
Morning: 14:00-16:00 UTC (7-9 AM Arizona)
Midday: 19:00-20:00 UTC (12-1 PM Arizona)
Evening: 02:00-04:00 UTC next day (7-9 PM Arizona)

5. Post Status Polling
After submitting a post, I automatically poll Blotato until it's confirmed as published, scheduled, or failed—you never have to ask "is it done yet?"
The system will:
Submit the post to Blotato
Receive a post ID
Automatically check status every 10-15 seconds
Continue until final status is reached:
✅ Published - Live on platform
📅 Scheduled - Queued for future posting
❌ Failed - Error occurred (will provide details)
You'll receive updates like:
"Post submitted, checking status..."
"Still processing..."
"Published successfully to Instagram!"
No action needed from you - just wait for confirmation.

6. Content Type Guidelines
Reflective Posts (Most Common - 60%)
When to use: Daily wisdom, philosophical reflections, mindfulness moments
Structure:
[Poetic opening - 1 line]

[Exploration - 2-3 sentences]

[Universal truth or invitation]

#SolMvmt #RelevantHashtags
Example:
Between the inhale and exhale, there is a moment of perfect stillness.

In that pause, you're neither holding on nor letting go. You simply are.

This is where clarity lives. This is where you meet yourself.

#SolMvmt #BetweenTheBreaths #MindfulLiving #YogaPhilosophy
Visual pairing: Soft focus imagery, nature, minimalist text overlays, meditation poses

Story-Based Posts (20%)
When to use: Sharing generational wisdom, personal narratives, transformative experiences
Structure:
[Story opening - 2-3 sentences]

[What it taught - 1-2 sentences]

[Universal application]

#SolMvmt #GenerationalWisdom #RelevantHashtags
Example:
My father walked miles in shoes with holes. Not for himself. For what he could bring home to us. For the life he never had but insisted we would.

Love isn't always loud. Sometimes it's quiet sacrifice in worn-out shoes.

When life gets hard, I remember: I am the answered prayer of my ancestors.

#SolMvmt #GenerationalWisdom #Legacy #IntentionalLiving
Visual pairing: Family photos, hands, walking paths, vintage aesthetics, golden hour lighting

Educational Posts (15%)
When to use: Teaching yoga philosophy, movement principles, practice tips
Structure:
[Concept introduction]

[Explanation/benefits - 2-3 sentences]

[Practical application]

#SolMvmt #YogaEducation #RelevantHashtags
Example:
Yoga isn't about touching your toes. It's about what you learn on the way down.

It's about showing up on the days you don't want to. It's about proving to yourself that you're worth the effort.

The mat teaches what the world often doesn't—that falling is part of the practice, not proof that you're failing.

#SolMvmt #YogaPhilosophy #LessonsFromTheMat #MindfulMovement
Visual pairing: Yoga poses, studio shots, close-ups of alignment, movement sequences

Invitation Posts (5%)
When to use: Promoting classes, events, workshops, outdoor sessions
Structure:
[Poetic opening - 1-2 lines]

**EVENT NAME**
📅 Day, Date
⏰ Time
📍 Location

[What to expect]
[What to bring]

Come as you are.

#SolMvmt #EventHashtags #LocalHashtags
Example:
Sometimes the best reset doesn't happen indoors.

**YOGA FLOW IN THE PARK**
📅 Sunday, March 24
⏰ 9:00 AM
📍 Discovery Park

Bring your mat, your water, and your willingness to begin again. All levels welcome.

Come as you are.

#SolMvmt #YogaInThePark #SanTanValleyYoga #OutdoorYoga
Visual pairing: Event location, mats on grass, outdoor settings, inviting spaces

7. Hashtag Strategy
Always Include (Core Brand - 3-5):
#SolMvmt
#YogaPhilosophy or #MindfulMovement
#BetweenTheBreaths (if relevant to series)
#PhoenixYoga or #ArizonaYoga
#SanTanValleyYoga (local)
Rotate Based on Content (5-8):
Yoga: #YogaFlow #YogaCommunity #YogaEveryday #YogaLife
Fitness: #FunctionalFitness #LagreeMethod #StrengthTraining
Outdoor: #OutdoorYoga #YogaInNature #ParkYoga
Philosophy: #MindBodySoul #IntentionalLiving #MindfulLiving #Presence
Content Series Specific (1-2):
#JoyBeyondGrief
#GenerationalWisdom
#LessonsFromTheMat
#GentleReminders
#SacredOrdinaryMoments
Event/Location Specific (when relevant):
#YogaArizona
#PhoenixWellness
Event name hashtag
Total per post: 10-15 hashtags (Instagram allows 30, but 10-15 performs better)

8. Caption Writing Best Practices
Voice & Tone Checklist:
✅ Contemplative and introspective
✅ Warm and accessible
✅ Personal yet universal
✅ Poetic but grounded
✅ Inviting, never pushy
What to Include:
Opening hook (question, observation, or story)
Body (exploration, teaching, or reflection)
Close (invitation, CTA, or question)
Emojis: 1-2 maximum, used intentionally
Hashtags: 10-15, placed at end
Line breaks for readability (every 2-3 lines)
What to Avoid:
❌ All caps (except event details like DATE, TIME)
❌ Excessive emojis
❌ Generic motivational quotes
❌ Sales-heavy language ("Limited spots!" "Book now!")
❌ Aggressive fitness language ("Crush it!" "Beast mode!")
❌ Trend-chasing that feels off-brand
Length Guidelines:
Instagram Feed: 100-180 words (1-2 phone screens)
Instagram Reels: 50-100 words (hook in first line)
Stories: 20-40 words (quick, digestible)
Mobile Readability Test:
Before posting, ask:
Does the first sentence hook attention?
Can you read it on a phone without scrolling too much?
Are there natural pause points (line breaks)?
Does it sound like a human, not a brand?

9. Visual Content Guidelines
Image Selection Criteria:
✅ Warm, natural lighting (golden hour preferred)
✅ Calm, uncluttered compositions
✅ Earthy, muted color palettes
✅ Authentic moments over posed perfection
✅ Close-ups: hands, breath, small details
✅ Wide shots: space, openness, invitation
Avoid:
❌ Overly polished, influencer-style imagery
❌ Busy, cluttered backgrounds
❌ Harsh lighting or aggressive colors
❌ Stock photo aesthetic
❌ Before/after comparison imagery
❌ Body-focused or comparison-inducing content
Text Overlay Standards:
Font: Clean sans-serif (Inter, Montserrat, Poppins)
Size: Large enough to read on mobile (65-85pt)
Color: White or charcoal (#3D3D3D) with shadow for contrast
Alignment: Centered or left-aligned, never right
Background: Use semi-transparent overlays if needed for readability
Brand Colors in Visuals:
Warm Beige (#E8DCC8)
Muted Gold (#A89968)
Soft Sage (#8B9C7C)
Charcoal (#3D3D3D)
Off-White (#FEFCF8)

10. Content Series Recognition
When creating content, identify which series it belongs to and use appropriate framing:
Series Name
Theme
Visual Cue
Hashtag
Between the Breaths
Stillness, transformation, pause
Minimalist, breath imagery
#BetweenTheBreaths
Joy Beyond Grief
Bittersweet, resilience, wholeness
Soft light, contemplative
#JoyBeyondGrief
Lessons from the Mat
Yoga philosophy in daily life
Yoga poses, studio shots
#LessonsFromTheMat
Generational Wisdom
Ancestral stories, legacy
Hands, paths, family themes
#GenerationalWisdom
Gentle Reminders
Simple truths, affirmations
Text-focused, circular designs
#GentleReminders
Sacred Ordinary Moments
Finding holiness in mundane
Coffee, laundry, daily life
#SacredMoments
When in doubt: Default to "Between the Breaths" series for reflective content.

11. Scheduling Best Practices
Optimal Posting Times (Arizona MST):
Monday-Thursday:
7:00-9:00 AM (morning routine time)
12:00-1:00 PM (lunch break)
7:00-9:00 PM (evening wind-down)
Friday:
8:00-11:00 AM (weekend planning mode)
Weekend:
9:00-11:00 AM (leisurely morning)
Weekly Content Mix:
Monday: Reflective post (start week with intention)
Tuesday: Educational post (yoga philosophy or practice)
Wednesday: Story-based post (Generational Wisdom)
Thursday: Gentle Reminder or Sacred Moments
Friday: Invitation post (weekend class/event) OR reflective
Weekend: Community-focused or behind-the-scenes
Consistency Over Frequency:
Better to post 3 high-quality posts per week than 7 mediocre ones
Maintain voice and depth over chasing algorithm
Build trust through reliability, not volume

12. Engagement & Community Guidelines
How to Respond to Comments:
Reply personally, not with generic responses
Use Kelly's voice (warm, thoughtful, present)
Ask follow-up questions when appropriate
Acknowledge vulnerability when people share deeply
Keep responses 1-3 sentences (concise but meaningful)
What to Share to Stories:
Behind-the-scenes studio moments
Nature walks or outdoor inspiration
Class reminders (day-of or day-before)
Reshares of student tags (with permission)
Quick reflections or morning thoughts
When to Use Polls/Questions:
"What brings you to the mat?" (engagement)
"Morning practice or evening practice?" (community insight)
"What theme should we explore next week?" (co-creation)
When to Tag or Mention:
Tag location for local discoverability
Tag music artists if using their tracks
Tag collaborators or guest teachers
Don't over-tag or spam

13. Content Workflow Summary
Step 1: Identify Content Type
Reflective / Story-based / Educational / Invitation
Step 2: Check Brand File
Read fabric_BRAND.md for voice, tone, audience
Step 3: Analyze Visual
Use view_file for images
Ask user for video description if needed
Step 4: Write Caption
Follow structure for content type
Include hashtags (10-15)
Add 1-2 emojis if appropriate
Read aloud to check flow
Step 5: Platform Requirements
Verify image/video specs match platform
Convert time to UTC for scheduling
Double-check caption length
Step 6: Submit to Blotato
Post via API
Automatic status polling begins
Confirm published/scheduled/failed
Step 7: Monitor & Engage
Respond to comments within 24 hours
Share to stories if relevant
Track performance for insights

How I Use This Skill
Whenever you ask me to post something for Sol Mvmt — whether it's an image to Instagram, a video to TikTok, or an event announcement — I follow this playbook to ensure the content is:
On-brand (voice, tone, visual style)
Platform-optimized (specs, timing, hashtags)
Contextually rich (never generic captions)
Properly scheduled (UTC conversion, optimal times)
Automatically confirmed (status polling until published)
I treat every post as a page in the larger Sol Mvmt story—contemplative, warm, grounded, and deeply human.

This skill ensures consistency, quality, and brand alignment across all Sol Mvmt social media content.
