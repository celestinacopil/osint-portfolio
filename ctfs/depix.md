---
layout: default
title: "Osint Industries | Depix"
---

<p class="eyebrow">CTF · CATEGORY</p>

# Depix

Osint Industries · Easy · September 26, 2026

## Overview

A passenger posted a heavily pixelated photo of their flight ticket online. The challenge is to recover three details using OSINT techniques: the passenger's full name, seat number, and arrival airport IATA code.

## Initial analysis

The only uncensored information on the ticket is the following : 
- 09JUN13 below the barcode
- PNR code: ONKMIF/AA
- American Airlines
- 49 U / LAX
- Printed in U.S.A

## Methodology

The first step was decyphering the layout of the ticket, in order to understand what does the visible information represent. For instance, 
is the 9th of June 2013 the date of departure, the day of acquisition or a code that just coincidentally resembles a date? does 49U / LAX mean anything? 
Is LAX the IATA of the airport of departure, maybe?

I answered these questions by looking up images of American Airline boarding passes (including a separate search for 2013). Two examples confirmed that the 3-letter code in the bottom right represents, indeed, the IATA of the departure airport. 

>First clue: LAX -> the airport of departure is Los Angeles International Airport.

The second step, for me, was to find out whether the PNR code contains any information. 
