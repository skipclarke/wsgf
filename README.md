# wsgf
Widescreen Gaming Forum

Public repository for any projects or discussions associated with the Widescreen Gaming Forum.

The WSGF offers an XML feed, which lists all the games in our database, along with their associated Steam ID (number).  We then list the different "grades" we've given for how each game supports widescreen, multi-monitor, ultrawide, and 4k UHD display configurations.  It also lists the path for the "Detailed Report" on the WSGF, along with the Node ID for the Drupal CMS.

The XML feed is located at http://www.wsgf.org/mgl/xml

The format of the individual entries is as follows: (see source for XML format)

`<node>`
  `<Title>A Valley Without Wind</Title>`
  `<SteamID>209330</SteamID>`
  `<Path>http://www.wsgf.org/dr/valley-without-wind/en</Path>`
  `<WideScreenGrade>A</WideScreenGrade>`
  `<MultiMonitorGrade>B</MultiMonitorGrade>`
  `<UltraWideScreenGrade>A</UltraWideScreenGrade>`
  `<Grade4k>Incomplete</Grade4k>`
  `<Nid>23705</Nid>`
`</node>`

Which results in this data string:

<node>
  <Title>A Valley Without Wind</Title>
  <SteamID>209330</SteamID>
  <Path>http://www.wsgf.org/dr/valley-without-wind/en</Path>
  <WideScreenGrade>A</WideScreenGrade>
  <MultiMonitorGrade>B</MultiMonitorGrade>
  <UltraWideScreenGrade>A</UltraWideScreenGrade>
  <Grade4k>Incomplete</Grade4k>
  <Nid>23705</Nid>
</node>

You can parse the the information on a per-game basis, by using the URL format http://www.wsgf.org/mgl/xml/SteamID

The link for the above game would be http://www.wsgf.org/mgl/xml/209330

You can then link back to the individual entry on the WSGF using the URL in the <Path> field, or with the following http://www.wsgf.org/node/nid.  For the above entry the link would be http://www.wsgf.org/node/23705

To display this information graphically in a program, each grade can be associated with a "medal".  Each of the "grades" has five associated results: A, B, C, D, and Incomplete.  A-D are correspond to Gold, Silver, Limited and Unsupported for display compatability.
