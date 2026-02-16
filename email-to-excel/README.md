Email Automation – Gmail to Google Sheets (Make.com)
Project Overview

This project demonstrates an automated email processing workflow built using Make.com.

The system monitors incoming Gmail messages, automatically replies to new emails, and logs all relevant data into Google Sheets.

Process Logic

Gmail module watches incoming emails.

The system checks Google Sheets using the Gmail ThreadID to prevent duplicate processing.

If the email thread is new:

A row is added to Google Sheets.

An automatic reply is sent.

The system logs:

Sender email

Subject

Date

Status

ReplySent (true/false)

ThreadID

MessageID

If the thread already exists:

No duplicate reply is sent.

Technical Concepts Used

Low-Code Automation (Make.com)

Gmail API integration

ThreadID-based deduplication

Router logic (conditional processing)

Status tracking & logging

Basic debugging and error handling

Outcome

The workflow ensures that each email is processed exactly once, preventing duplicate replies and maintaining a structured log for tracking and auditing.
