# raven-wiki

html back ups of the raven.wiki domain

Wiki is run on a standard mediawiki installation, with MobileFrontend, Youtube and WikiSEO extensions

# Custom settings in addition to standard LocalSettings.php #

$wgLogo = "/w/images/Raven_black_sm.png";

$wgGroupPermissions['*']['edit'] = false;

$wgGroupPermissions['*']['move'] = false;

$wgGroupPermissions['*']['createpage'] = false;

$wgGroupPermissions['user']['edit'] = false;

$wgGroupPermissions['user']['move'] = false;

$wgGroupPermissions['user']['createpage'] = false;

$wgGroupPermissions['sysop']['edit'] = true;

$wgGroupPermissions['user']['createpage'] = true;

$wgGroupPermissions['Write']['edit'] = true;

$wgGroupPermissions['Write']['createpage'] = true;

$wgArticlePath = "/wiki/$1";

$wgUsePathInfo = true;

$wgGenerateThumbnailOnParse = false;

wfLoadExtension( 'YouTube' );

$wgEnableUploads  = false;

$wgScriptExtension = ".php5";

wfLoadExtension( 'MobileFrontend' );

$wgMFAutodetectMobileView = true;

wfLoadSkin( 'MinervaNeue' );

$wgDefaultSkin = 'vector';

$wgMFDefaultSkinClass = "SkinVector";

$wgShowExceptionDetails = true;

wfLoadExtension( 'WikiSEO' );

# allowing external images - not currently allowing image uploads

$wgAllowExternalImages = true;

$wgAllowImageTag = true;

