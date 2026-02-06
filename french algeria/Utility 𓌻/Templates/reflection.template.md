---
aliases: reflection
tags: reflection
status: draft
date: <% tp.file.creation_date() %>
title: <% tp.file.title %> 
---

<%*
	let title = tp.file.title 
	if (title.startsWith("Untitled")) {
		title = await tp.system.prompt("Title");
		await tp.file.rename(`${title}`);
	}
%>
# <%* tR += `${title}` %>

## Summary
>[!tip]- Briefly describe the video’s main idea or argument. 
>- Keep it short, 2–3 sentences.

I/P: 

---
## Thoughts
>[!tip]- Write your personal reactions. 
>What resonated with you? Did anything surprise or challenge you?

I/P: 

---
## Key Takeaways
>[!tip]- List memorable points, insights, or lessons you want to remember. 
>You can include quotes or timestamps.

I/P: 

---
## Notes / Links
>[!tip]- Any extra ideas, observations, or related resources. 
>Include links to other notes or references.

-