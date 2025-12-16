Directory Structure
===

Theme names may consist of A-Z (mixed case), 0-9 and dashes. No other characters are permitted.

Each theme needs to be placed within its own directory with the name of the theme. It should contain the following files:

    ThemeName\ThemeName.css   //The main theme file
    ThemeName\ThemeName.less  //(Optional - the original if LESS is used)
    ThemeName\info.json       //Metadata about the theme (See below)
    ThemeName\preview.png     //A 420x350px preview of the theme based on the theme preview from within AMP

info.json
===

```
{
	"Name": "ThemeName",
	"Version": "1.0",
	"UpdatedDate": "2024/08/23",
	"Description": "A description of my theme,
	"URL": "https://example.org",
	"Author": "Author Name",
	"Tags": ["Contributor", "Example"]
}
```

`Name` is the name of the theme exactly matching the theme directory and css file name.
`Version` is a semver version, this isn't currently used for anything important.
`UpdatedDate` is the date the theme was updated in YYYY/MM/DD format.
`Description` A user-facing description of the theme and how it looks, and who may benefit from it.
`URL` is an address for the author (for example a personal website, github page, etc)
`Author` is the name(s) of the author(s), comma separated if there are multiple.
`Tags` is a list of user-defined tags. All third party themes must have the tag "Contributor", other tags can include things like "Dark", "Light", "Accessible", or any other tags which define the theme. These tags are used to build the top-level category lists within the store page.

preview.png screenshots
===

These screenshots are shown within the store page in AMP.  See the [Coffee Example](https://github.com/CubeCoders/AMPThemes/blob/main/Coffee/preview.png) for how they should look - they are obtained by previewing a theme within AMPs store and reducing the size of the preview page, and then cropping to the desired elements only.
