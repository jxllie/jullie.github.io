<!DOCTYPE html>
<head>
<meta charset="UTF-8">
<title>{Title}</title>
{block:Description}
<meta name="description" content="{MetaDescription}" />
{/block:Description}
<link rel="shortcut icon" href="{Favicon}">
<link rel="alternate" type="application/rss+xml" href="{RSS}">
 
<style type="text/css">
 
/* CSS */
 
</style>
</head>
 
<body>
 
{block:Description}{Description}{/block:Description}
<a href="/">home</a>
<a href="/ask">ask</a>
 
{block:Posts}
 
{block:Text}
{block:Title}{Title}{/block:Title}
{Body}
{/block:Text}
 
{block:Quote}
{Quote}
{block:Source}{Source}{/block:Source}
{/block:Quote}
 
{block:Link}
<a href="{URL}">{Name}</a>
{block:Description}{Description}{/block:Description}
{/block:Link}
 
{block:Chat}
{block:Title}{Title}{/block:Title}
{block:Lines}
<div class="{Alt} user_{UserNumber}">
{block:Label}{Label}{/block:Label}: {Line}
</div>
{/block:Lines}
{/block:Chat}
 
{block:Answer}
{Asker}{Question}{Answer}
{/block:Answer}
 
{block:Photo}
{LinkOpenTag}<img src="{PhotoURL-400}" alt="{PhotoAlt}"/>{LinkCloseTag}
{/block:Photo}
 
{block:Photoset}
{Photoset-400}
{/block:Photoset}
 
{block:Video}
{Video-400}
{/block:Video}
 
{block:Audio}
{block:AlbumArt}<img src="{AlbumArtURL}">{/block:AlbumArt}
{AudioPlayerWhite}
{block:TrackName}{TrackName}{/block:TrackName}
{block:Artist}{Artist}{/block:Artist}
{block:Album}{Album}{/block:Album}
{/block:Audio}
 
{block:Caption}{Caption}{/block:Caption}
 
{block:Date}<a href="{Permalink}">{TimeAgo}</a>{/block:Date}
{block:NoteCount}<a href="{Permalink}">{NoteCountWithLabel}</a>{/block:NoteCount}
 
{block:HasTags}{block:Tags}
<a href="{TagURL}">{Tag}</a>
{/block:Tags}{/block:HasTags}
{block:RebloggedFrom}
<a href="{ReblogParentURL}">{ReblogParentName}</a>
{/block:RebloggedFrom}
{block:ContentSource}
<a href="{SourceURL}">{SourceTitle}</a>
{/block:ContentSource}
 
{block:PermalinkPage}
{block:NoteCount}
{block:PostNotes}{PostNotes}{/block:PostNotes}
{/block:NoteCount}
{/block:PermalinkPage}
 
{/block:Posts}
 
{block:Pagination}
{block:PreviousPage}<a href="{PreviousPage}">previous</a>{/block:PreviousPage}
{block:NextPage}<a href="{NextPage}">next</a>{/block:NextPage}
{/block:Pagination}
 
</body>
</html>
