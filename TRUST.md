# What Lumen does with your work

Most plugins ask you to trust them. This one tells you what happens instead.

## What it is

Six skills install into your agent. Each does its work on your machine, then asks a hosted service whether the result is ready before handing it over.

The point is that producing something and producing something good are different claims. Only the second one gets checked here.

## What leaves your machine

A request carries the artifact being checked and the evidence that check needs. Your credentials and unrelated files stay where they are.

Skills are told not to search your workspace before they know what you are asking for.

## What is kept

Submitted content stays out of storage. What gets recorded is how many checks ran, not what was in them.

Memory is the exception. A preference you explicitly approve gets stored so later runs can use it. Removing it takes one request.

## Where it goes

One host over HTTPS, through the client bundled with each skill. Nothing else receives your work, and no third-party analytics sit in the path.

## Your key

The key authenticates your account and is stored locally by the bundled client. It travels only as an authorization header.

Ask your agent where it lives and you will get an answer, though the value itself stays unprinted.

## What is held back

How the scoring works is server-side and stays that way. That is the only withheld thing, and deliberately so.

Skills answer plainly when asked what is running or where data goes. A skill that dodges that question is a bug worth reporting.

## Without a key

The skills still run and return unchecked output, clearly labelled. Checking is the part that needs an account.

## Questions

Write to hello@siraj.ai.