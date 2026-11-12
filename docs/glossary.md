# Glossary

The four terms you meet most often in Pocket Timer.

## Session

A session is a block of focused work. You start one with `pocket start`. It lasts 25 minutes by default; change it with `session_minutes` (see [session length](configuration.md#session-length)).

## Break

A break is a rest between sessions. You start one with `pocket break`, and it lasts 5 minutes. Breaks never count toward your [daily goal](#daily-goal).

## Daily goal

The daily goal is how many sessions make a full day. It is set with `daily_goal = 8` (see [daily goal](configuration.md#daily-goal)), and `pocket today` shows your progress.

## History

The history is the record of your sessions and breaks. It lives in `~/.pocket/history.jsonl`, one line per session or break (see [where your history is stored](faq.md#where-is-my-history-stored)).

Back to [the index](index.md).
