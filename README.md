## LinkedIn Post & Image Automation with n8n

This project is an n8n workflow that automates the creation of LinkedIn posts and generates branded images with AI. The workflow takes user input from a form, generates a LinkedIn-ready caption and image prompt, creates the image, and logs both the post text and image URL into a Google Sheet for record-keeping.

## 🚀 Features

Form-triggered input → easily create posts from a simple form.

AI-powered LinkedIn Post Generator → generates engaging captions using OpenAI.

AI-powered Image Prompt Generator → converts context into creative image prompts.

Image Generation → produces images dynamically (e.g., via DALL·E or Stable Diffusion).

Cloudinary Upload → stores images and returns hosted URLs.

Data Logging → automatically appends post text + image URL into Google Sheets.

Scalable → ready for expansion into auto-publishing on LinkedIn.

## 🛠️ Tech Stack

n8n
 – workflow automation

OpenAI – AI-based text & image prompt generation

Image API – DALL·E / Stable Diffusion (configurable)

Cloudinary – image hosting & delivery

Google Sheets – stores post text and image URLs

## 📂 Workflow Overview

On Form Submission → user submits post idea.

LinkedIn Post Agent → generates LinkedIn-style caption text.

Image Prompt Agent → produces a creative prompt for the image.

Create Image → generates image from AI.

HTTP Request to Cloudinary → uploads generated image and returns URL.

Merge Node → combines post text + image link.

Append Row in Google Sheet → stores both for tracking and future publishing.

## ⚡ How to Use

Import workflow.json into your n8n instance.

Configure credentials:

OpenAI API key

Cloudinary API key & secret

Google Sheets API credentials

Connect your Google Sheet (columns: Post Text, Image URL, Timestamp).

Deploy the workflow → fill out the form → generated post + image URL will drop into your Sheet automatically.
