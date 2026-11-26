# Changelog

Every Offrun release, newest first. Download the latest from [offrun.dev](https://offrun.dev/download/?utm_source=github&utm_medium=referral&utm_campaign=repo-2026-11); the same notes are at [offrun.dev/changelog](https://offrun.dev/changelog/).

## 6.6.5, 13 November 2026

- Pick the login in the model menu, and Cmd/Ctrl-Shift-M opens the model picker. Claude chats keep working after a login switch.
- Chats group plan notes under their steps, show each shell command, and draw the files an answer ends on as cards.
- Mark a chat as unread from its menu or with Cmd/Ctrl-Shift-E. The workspace switcher shows each workspace's agent status.
- Agents can use Offrun's browser or their own (Settings). Preview tabs keep their scroll place, and Cmd/Ctrl-Shift-T reopens a closed tab.
- Background agents stay alive across turns, and agents can fix and rerun a failed job up to five times.
- A waiting approval shows on the working line, and a switch card appears when Claude runs out of usage credits.
- A cleaner look: chat tools in clearer groups, a taller message box, a wider live dictation box and smaller buttons.
- Fixes cover failed OpenCode turns, dictation text with app zoom, new chats that closed at once and project folders renamed outside Offrun.

## 6.6.4, 9 November 2026

- Choose Auto and Offrun picks the AI model.
- You can add a message while an agent is working. And chat will not get interrupted.
- When you reopen a chat, you can carry on where you left off.
- Try the new Light theme
- You can now search Settings to find an option.
- Offrun shows when you need to sign in again and explains sign-in errors.
- Pastes longer than 10 lines take less space in the message box. Hover to preview the text, or double-click to expand it.
- Save bookmarks in Preview, edit Markdown text beside a live preview, and drag browser tabs to reorder them or open them in a separate window.
- Bug fixes and optimizations.

## 6.6.3, 25 October 2026

- New Gemini models show in the Agents model picker on their own as soon as agy offers them, at the top of the Agy group. Before, each one had to be added by hand.
- Sending a message starts at once. Before, it could wait several seconds while your connectors reloaded.
- The X and zoom buttons on a large diagram preview work again. Before, only Esc closed it.
- When an agent changes files in another project folder, the changes card and Changes tab now show those files too.
- Background jobs an agent starts can now run for up to 24 hours, the same as background tasks. Before, they stopped after six hours.

## 6.6.2, 23 October 2026

- Connectors keep working after heavy use. Before, a long list of requests whose answer never arrived could block every new connector request with "Connector request failed".
- Connector request history now stays in memory only, so the connectors file on your computer is much smaller and old requests are never sent again after a restart.
- An agent that checked its own background job and found it finished now shows its final answer as an answer, not as a folded progress note.
- Changed-file cards keep each line in green or red when you scroll sideways through a long line.

## 6.6.1, 21 October 2026

- When an agent changes files, its answer now ends with a card listing each changed file and its added and removed lines. Open diff shows every file of that turn in a Changes tab beside the chat.
- Code changes now show by default. Turn them off in Settings > Agents > Show code changes.
- Connectors: choose what agents may do in each connected app, by kind (see, create, change, delete) or action by action. Offrun refuses any action you leave off.
- Dictation can use agy as an optional speech engine, in Settings > Dictation. agy sends audio to Google; the default Apple engine keeps it on your Mac.
- Pressing Fn while Offrun is full screen no longer slides the screen to the Desktop.
- Settings lists every agent's sign-in, with a link to its install guide and a Refresh button. A new switch stops sharing crash and error reports.
- A file or page an agent opens now shows in that chat's own preview, and tapping an agent notice puts the cursor straight into the reply box.
- Idle agents release memory sooner, and the Help ticket form has clearer topics.

## 6.6.0, 19 October 2026

- Each project, worktree and folder now keeps its own browser, terminals and tasks. Pin a browser tab to keep it first in every project.
- Code changes now show right in the chat, and agents can draw ER diagrams in their answers.
- New notifications bell: see what your agents finished, with a dot for anything you have not seen yet.
- Home shows Grok and Muse plan usage. Connectors shows each account's email, with logos for 54 more apps, and Jira Reconnect keeps your company address.
- Sign-in pop-ups in the preview browser, like Continue with Google, now work. You can also try English learning on YouTube in the preview.
- Reviews now cover repos your agent changed outside the chat folder. Updates now show in the sidebar with a progress ring.
- Fixes: Enter with Korean and other input methods finishes the character instead of sending, folders whose names end in a space work, and empty bars drag the window.
- Lighter: less memory use, a smaller app, and usage syncs once an hour instead of every 30 seconds.

## 6.5.1, 14 October 2026

- Agent chats started before Offrun was renamed could not use Offrun commands (memory, plans, skills, the preview browser): they failed with "No such file or directory". They now repair themselves on the next message.
- Projects set up under the old Offloop name no longer run a broken memory hook on every Claude prompt. Offrun replaces it with the current one.

## 6.5.0, 14 October 2026

- Offrun now installs as Offrun.app instead of offrun.dev.app. Your settings and data carry over. If you pinned Offrun to the Dock, drag the new app there once.
- Muse Code is now available as a fifth agent.
- Agents can draw flowcharts in their answers, with a preview you can zoom.
- Switch between recent chats with Command and the ` key. Streamed replies now fade in word by word.
- The Artifacts list now shows only what a chat made, not every file it touched.
- Plus > File Explorer can attach several files at once, and long questions show a four-line preview.
- Dictionary: Edit and Delete are on every row, and voice samples are gone. The Ubuntu theme now ships its own Ubuntu fonts.
- A redesigned provider sign-in dialog, a Settings gear in the model list, and alignment fixes across the Agents sidebar, previews and notifications.

## 6.4.0, 11 October 2026

- Dictation now runs on Apple's on-device speech engine. No speech or AI model downloads, and it uses about 1 GB less memory.
- Dictation needs a Mac with Apple silicon on macOS 26 or later. On older Macs, Settings explains why it is off.
- While you hold the key, a small pill sits at the bottom of the screen and your words appear live in a box above it. Nothing stays on screen otherwise.
- Text is cleaned up by fast rules: lists, emails, web addresses, fillers and "no wait" corrections. Apple's engine writes dates, money and numbers.
- The dictation Memory screen has been removed. Your dictation history stays on the Dictation page.
- The main window can now shrink to 720 by 440.
- Holding Backspace in the agent composer now deletes words at a steadier pace.
- A folder added to a project with New folder gets Git set up, and approved reviews show a tick.

## 6.3.0, 10 October 2026

- Reply options now appear as numbered cards you can pick with a number key, and they stay usable after a background agent reports back.
- Steer now reaches an agent even while its helpers are working, and you can cancel a queued message before it is sent.
- Tool calls are easier to read: each one sits in a tidy box that shows its command or file path once, in the same code font as your answers.
- Tasks now groups work into one card per chat and shows running agents the moment they start. Failed tasks no longer count in the top bar.
- More room for the chat: focus mode can hide the Projects pane, the app menu and Projects pane each have their own hide button, and panels animate as they open and close.
- Press Cmd/Ctrl-Shift-T to reopen the last closed tab. Closing a blank Untitled chat removes it, and typing anywhere in a chat goes straight to the message box.
- Safer deletes: removing your account or a project folder now lists what goes and what stays, and asks you to type to confirm.
- Schedules that came due while the computer slept now run when Offrun wakes, background shells no longer stop after 30 minutes, and Hindi dictation was removed, saving a 250 MB download.

## 6.2.0, 9 October 2026

- New agent at the top of the sidebar starts a chat right away in a Default project, and first-time users get a welcome with four starters.
- Scheduler: agents can do things at a set time, use your connected apps, and send a notification after every run.
- Connect any of 1,385 apps, including apps where you paste your own key, with logos and smooth scrolling.
- Grok Build joins as a fourth agent, agy offers Claude, GPT-OSS and Gemini Pro models, and the model picker adds coding rankings, search and sort.
- Calmer chats: one Activity fold per turn, a long answer's question stays pinned on top, tabs show a dot when an answer is ready, and Ubuntu marks your messages in orange.
- Artifacts replaces the Changes tab and previews what agents made. The preview shows Word files, zooms with a trackpad pinch and opens web links from answers.
- Pin projects to keep them on top, delete projects with a confirmation, keep per-chat Notes the agent can read, and delete your account from Settings.
- Steadier agents: a chat stays usable while background subagents run, servers run as background tasks in the top bar, and a clear Sign in message shows when a login runs out.

## 6.1.0, 4 October 2026

- New Codex and Claude models appear in the model picker on their own, and Codex Ultrafast speed shows up when your account offers it.
- Agents start faster: fewer cold starts for Claude, Codex and agy, and each chat keeps its own warm agent ready.
- Build and Planner modes size their work to your request and post short progress updates while they work.
- More reliable turns: Codex and Claude turns end at the right moment, and a stuck Working clock or Stop button now clears itself.
- Chats open faster by loading the latest five exchanges first, and a new chat is named from your first message.
- Plan cards show a live clock on the running step, and long jobs show how far they have got.
- Delete chat now asks first in a themed popup, the composer is ready to type when an answer ends, and attachment previews line up.
- Notifications stay on screen for 15 seconds, connectors show logos for 71 more apps, and the app uses less memory while you are away.

## 6.0.9, 3 October 2026

- Drag a project onto another to move its folder inside it. Chats, memory, folders and worktrees move with it, and nested projects fold open and shut with their parent.
- Pick a look for the whole app in Settings > General: Default, Ubuntu or Terminal.
- Connectors such as Gmail, Google Calendar and Slack now work on every plan, including Free.
- Folders and worktrees can be dragged into any order inside a project, and an agent whose background job is still running shows as working.
- Every agent now follows the rules and skills you wrote for the others (CLAUDE.md, AGENTS.md, GEMINI.md), and the reviewer checks changes against them.
- Esc stops the running agent even while the preview is open, and Shift+Tab changes the agent effort.
- Preview: a typed address opens there, a narrow window shows the preview full width with Show chat to swap back, and dragging the empty tab bar moves the window.
- Dictation Fast mode frees its formatting model from memory, and agents now list proof files as links that open in the preview.

## 6.0.8, 1 October 2026

- Agents: Claude, Codex and agy can open and drive pages in Offrun's preview panel, and you can take over at any time.
- Agents: a new picker sets the model, effort and fast mode for the agent and the reviewer, with models grouped by Anthropic, OpenAI and Google.
- Agents: type / to use a skill from any agent, and move a chat to another folder or worktree; its terminal and dev servers follow it.
- Agents: big jobs show a live plan card, and you can watch the reviewer work and ask it to review again.
- Agents: live token counts for every agent, and closing a tab while an agent works lets the work finish first.
- Preview: edit CSV tables, view PowerPoint decks, pinch to zoom images, and expand the preview over the chat.
- Setup: agents come first and dictation is optional. Connectors now connect through Composio.
- Fixes: the low battery warning shows below 5%, and the sign-in screen is cleaner.

## 6.0.7, 28 September 2026

- Agents: Claude replies faster from the second message on, because it stays ready between messages.
- Agent chat: replies no longer jump up and down while they are written, and a sent message glides into place.
- Agents: a Claude background helper that gets cut off now says so, instead of ending with no answer.
- Agents: asking for a status while a long job runs gets a visible reply.
- Agent chat: pick an answer by clicking a choice, and a context meter in the composer shows how full the chat is.
- Updates: the app asks before it downloads a new version.
- Home: stats switch by signed-in account, and the bars show their figures on hover.

## 6.0.6, 28 September 2026

- Agents: large chats no longer flicker while an answer is being written.
- Agents: every agent has a face. An idle agent sleeps, and an error or question you have already seen stops calling you.
- Agents: Yes on a go-ahead question sends at once, and No closes the box.
- Agents: the token count under each answer shows the new input and the output, not the reused prompt cache.
- Agent chat: file names link only when the file exists, opening a preview keeps you on the newest line, and headings are never smaller than the text.
- Dictation: the pill shows over a full-screen Offrun window, and the pill, live text and card match the new design.
- Remote access is rebuilt on the new design, with a phone icon.
- Polish: worktrees fold open on a gentle spring, and the line beside the side rail shows on every screen.

## 6.0.5, 27 September 2026

- A fresh look: Home, Dictation, Help and setup are rebuilt on one design, with window glass on every screen.
- Agents: run up to four chats side by side, each with its own composer.
- Agents: when one agent runs out of usage, Offrun offers another one to carry on.
- Agents find your project notes by meaning, not just matching words. A small search model (about 35 MB) downloads in the background the first time you use an agent, and stays on your computer.
- Agents: two simple modes, Build and Planner. Escape stops a turn, and Copy chat is in the right-click menu.
- Apple Notes works as a connector again, and Excel workbooks open in the Agents preview.

## 6.0.4, 27 September 2026

- The sidebar and menu bar now show the new app name too.
- Your projects, chats, settings and microphone and accessibility permissions all carry over untouched.
- If you keep the app in your Dock, drag it back once from Applications after this update.

## 6.0.3, 25 September 2026

- The app has a new name in Finder, Spotlight and the Dock, and the old Offloop name is gone.
- Your projects, chats, settings and microphone and accessibility permissions all carry over untouched.
- If you keep the app in your Dock, drag it back once from Applications after this update.

## 6.0.2, 25 September 2026

- Agents: open an agent's browser links in the in-app preview.
- Agents sidebar: a running dot on a project row.
- No light flash at launch. The window paints dark from the first frame.
- Screenshots: Copy on the markup sheet, by button or Cmd/Ctrl+C.
- Chat panel: wider side margins that line up with the composer.
- Token counts show in billions past 1000M.

## 6.0.0, 25 September 2026

- Offloop is now Offrun. Your projects, chats and settings carry over.
- Agents radio: reconnects when a live stream stalls.
- Agents: a background agent's report folds shut once it finishes.
- Dictation: the on-screen bar recovers after the computer wakes, and windows open where they should.
- Agents: fixes to moving through the composer and to the spacing of the Agents header.

## 5.1.6, 23 September 2026

- Agents: the computer stays awake while agents and their reviewers are working.
- Agents: a ChatGPT-style neutral theme, folded activity and a microphone button in the composer.
- Agents: the review row folds open to show the reviewer's steps and words.
- Agents: background helpers no longer light up the working pane, and Stop also stops the reviewer.
- Dictation: the bar starts on the display under your cursor.

## 5.1.5, 19 September 2026

- Home page fills the width with separate counter cards, weekly stats above usage, and a loading shimmer.
- Focus mode for the app, an independent frosted-glass transparency slider for Agents, and bulk-close for agent chat tabs.
- Agent alerts are cards with an Open button, and agent progress shows before the turn finishes.
- Connectors run reads and writes immediately with no approval step, plus a new local Telegram connector.
- Fixes: menu-bar screen placement, mic recovery after background wakes, preview alignment at non-default zoom, and Terminal glass message tint.

## 5.1.1, 17 September 2026

- Connectors: link Gmail and Google Calendar to your agents, with no keychain prompt.
- Agents chat: Engineer mode, paste images and files, mark up a screenshot before sending, Cmd/Ctrl-W closes a tab, Up and Down recall sent messages, Tab takes a suggested reply.
- Agents: Default, Ubuntu and Terminal themes, the effort control follows the chat's model, and the Agents tab opens without a flash.
- Insights shows agent token usage, and the backend stopped dialog no longer freezes after the computer sleeps.

## 5.1.0, 15 September 2026

- Agents keep going through long multi-step work instead of stopping after three steps, and the reviewer no longer pauses in long chats.
- Agents can transcribe audio files, including WhatsApp voice notes.
- Settings > General has a Send logs button that sends your Offrun log files to the team.
- The sign-in screen stays in the dark theme.

## 5.0.9, 14 September 2026

- Dictation no longer goes silent after the microphone restarts during a session. A key press while it recovers now shows that Offrun is getting ready.
- Agent reviews look only at what the agent changed in that turn, skip turns that changed no files, and show each finding on its own lines.
- The turn markers down the left of an Agents chat no longer cover the text on wide windows.

## 5.0.8, 13 September 2026

- Switching Spaces no longer pulls you back to Offrun. Only opening it from the Dock or the menu brings the window forward.
- Dictation keeps working after long sessions: an audio recovery lock-up and a background memory leak are fixed.
- A green or red dot at the bottom left shows whether dictation is ready.
- Type /context in any Agents chat to see what fills the context window.
- The model list recovers on its own when an agent CLI was not ready at startup, and a failed turn shows its error once.
- Clicking Send works the same as pressing Enter, and files dropped anywhere on the chat attach to the message.
- Transcribe takes several dropped audio files at once and lists your saved transcriptions.
- New Solid, Frosted and Clear themes in dark and light. Hold the theme icon to set how see-through the chat is.
- Cmd/Ctrl+R starts and stops the Agents radio, and Cmd/Ctrl+W in the preview closes just that tab.

## 5.0.7, 11 September 2026

- Saved environment variables no longer go through the system keychain, so the app never asks for your login password.
- Scrolling up while an agent types now holds, whatever the distance, with a Jump to latest pill to come back.
- The working line shows the CLI's real token count for the turn.
- Answers use the same text rhythm as ChatGPT, and the message-edit box is a plain bubble with Cancel and Send.
- A run of tool calls folds into one Activity block, and agy system blocks are folded away.
- The strip above Projects drags the window, and the remote dialog has a stop glyph and a Copy pairing link button.

## 5.0.6, 11 September 2026

- Offrun Remote: pair your phone with a QR code and run the selected project's agents from its browser.
- Long jobs: an agent can hand a long command to a managed job with its own deadline and saved status, and the chat picks up when it settles.
- Environment variables per chat: give an agent a key or a URL without pasting it into the message. The value is masked in the answer.
- Background agents no longer lose the final answer, and the working line lists the agents still out.
- Status dots per chat, rename projects and workspaces, drag the window by the Agents top bar, and the message box takes focus when a chat opens.
- A popup warns below 2 percent battery. Notification settings show what your system allows, and a Codex reply is announced once.
- An update that drops mid-download resumes from the bytes it already has.

## 5.0.5, 11 September 2026

- An agent turn has no time limit any more: it runs until it finishes or asks, and only Stop ends it.
- Tool calls fold away once a turn is done, and open again with one click.
- The reviewer shows itself under the answer while it works, with a stop of its own and a thirty minute limit it names.
- Codex launches on the Node it was installed with, whatever else is installed.
- The context ring uses the window the model really has, so a long thread is no longer compacted early.
- Shared memory reaches Claude again. A missing file kept it out of 5.0.3 and 5.0.4.
- Gemini is told its time limit, and a turn it cuts short says so instead of ending empty.

## 5.0.4, 10 September 2026

- Gemini turns are no longer cut short at five minutes, and a turn that does stop at its limit says so in the chat.
- You can watch the agent think while it works, instead of a word and a timer.
- Chat titles, memory notes, handovers and compaction run on a lighter model, so your plan's limits go further.
- The reviewer reads every repository in a workspace, is told what was asked, and gets ten minutes.
- Switching a chat to another agent hands over a short note instead of the whole conversation.

## 5.0.1, 8 September 2026

- The Agents workspace runs your coding agents inside Offrun, with saved chats you can reopen, rename and fork.
- Keep more than one login for an agent, and Offrun moves to the next one when a rate limit hits.
- Your computer stays awake while an agent is working, and sleeps again below 10 percent battery.
- A calendar in the Agents bar shows how much of the year is gone.
