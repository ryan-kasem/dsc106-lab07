# Lab 7 demo video script (aim for ~55 seconds)

**Setup before recording:** open https://ryan-kasem.github.io/dsc106-lab07/ in Chrome, wait for the circles to load, put the slider on "(any time)", and zoom to Cambridge/Boston. Record the screen with Zoom or QuickTime and export as .mp4.

| Time | Do this on screen | Say this |
|---|---|---|
| 0:00–0:08 | Show the full page | "This is Bikewatching, my Lab 7 map of about 260,000 Bluebikes rides in Boston and Cambridge from March 2024, built with Mapbox and D3." |
| 0:08–0:16 | Drag to pan, scroll to zoom in and out | "It's a Mapbox map, so I can pan and zoom. The green lines are the Boston and Cambridge bike lanes, loaded as GeoJSON layers." |
| 0:16–0:24 | Point at the circles while zooming; they stay in place | "Each circle is a station, drawn in an SVG layer on top of the map with D3. It stays lined up when I zoom because I re-project with map.project on every move." |
| 0:24–0:30 | Hover a big circle near MIT so the tooltip shows | "Circle area shows total traffic on a square-root scale. Hovering shows the exact trips, departures and arrivals." |
| 0:30–0:42 | Drag the slider to ~8:30 AM, then to ~5:30 PM, then back to the far left | "The slider filters to trips within an hour of the chosen time. At 8:30 AM, Kendall and downtown turn orange, meaning more arrivals. At 5:30 PM that orange disappears, and those stations go back to balanced or blue as people head home. All the way left goes back to any time." |
| 0:42–0:47 | Point at the legend | "The legend shows the three flow colors: more departures, balanced, and more arrivals." |
| 0:47–0:57 | Stay on the map | "The most interesting thing I learned was performance. Filtering 260K trips on every slider move was laggy, so I pre-sorted trips into 1,440 buckets, one per minute, and now each update only reads about 120 buckets." |

**Tips**
- Total speaking is about 160 words. That fits in under 60 seconds at a normal pace, but do a timed run first.
- Tooltips use the browser's built-in title, so keep the mouse still on the circle for about a second.
- If you go over time, cut the 0:16–0:24 line down to: "Each circle is a station, drawn with D3 on top of the map."
