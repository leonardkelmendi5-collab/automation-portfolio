Email Automation – Gmail & Google Sheets (Make.com)
Project Overview

This project demonstrates an automated email processing workflow built using Make.com.

The system monitors incoming Gmail messages and ensures that each email thread is processed only once.

Process Logic

Gmail watches incoming emails.

The system checks if the ThreadID already exists in Google Sheets.

If the thread is new:

Email metadata is logged.

An automatic reply is sent.

Status is updated.

If the thread already exists:

No duplicate reply is sent.

Technical Concepts Applied

Event-driven automation

Thread-based deduplication

Idempotent processing

State tracking (NEW → REPLIED → ERROR)

Logging and audit trail

Challenge & Solution

Initially, using "Send an email" created new threads and broke the deduplication logic.

The issue was solved by switching to "Reply to an email" and correctly mapping the Gmail ThreadID.

Purpose

This project was created as a self-learning exercise to understand process automation and integration logic before starting a professional training program.
