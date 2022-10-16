<style>
/* Created by Apostol Apostolov. V.1.041 7th of March 2020.  */
/* For support, join Grit and Glory Discord at https://discord.gg/ZDtCmhm */
/* Please do not remove this message. It allows people who copy the template from your work get dev support. */
/* It also helps others find newer version of the template by comparing the version number with their own    */

/* Fonts */
@import url('https://fonts.googleapis.com/css?family=Eczar:800|Roboto+Condensed|Tauri|Teko:500|Changa+One|Gelasio|DM+Serif+Text:400i&display=swap'); /* Loads fonts from Google Web Fonts. Add additional @import if you license web fonts from elsewhere (such as from Monotype) */

/* Proper Printing */
@media print { .phb { height: 279.4mm; width: 215.9mm; } }

/* Background */
/* Sets two backgrounds. First image is the image margin column on each page, the second is the Pathfinder signature parchment. You can change the image margin depending on the content of your book but I suggest that you use the Imgur image I am using and just change the picture in the upper frame. I had to redesign the whole image margin and just using one from a Paizo PDF will not fit the whole length. On odd pages the parchment is horizontall flipped to emphasize odd and even pages. */
.phb{ background-image: url('https://www.gmbinder.com/images/2B04yOU.png'), url('https://www.gmbinder.com/images/Nrkf77U.jpg'); background-size: 97px, 822px; background-repeat:no-repeat; }
.phb:nth-child(odd){ background-image: url('https://www.gmbinder.com/images/8hcD3pd.png'), url('https://www.gmbinder.com/images/EABESdy.png'); background-size: 97px, 820px; background-repeat:no-repeat; background-position:right, center; } 

/* Cover */
.cover-title { font-family: 'Eczar', sans-serif !important; color:#4E0707; border-color:#EFCD98; border 10px; text-shadow: 1px 1px 0 #EFCD98, -1px 1px 0 #EFCD98, 1px -1px 0 #EFCD98, -1px -1px 0 #EFCD98, 0px 1px 0 #EFCD98, 0px -1px 0 #EFCD98, -1px 0px 0 #EFCD98, 1px 0px 0 #EFCD98, 2px 2px 0 #EFCD98, -2px 2px 0 #EFCD98, 2px -2px 0 #EFCD98, -2px -2px 0 #EFCD98, 0px 2px 0 #EFCD98, 0px -2px 0 #EFCD98, -2px 0px 0 #EFCD98, 2px 0px 0 #EFCD98, 1px 2px 0 #EFCD98, -1px 2px 0 #EFCD98, 1px -2px 0 #EFCD98, -1px -2px 0 #EFCD98, 2px 1px 0 #EFCD98, -2px 1px 0 #EFCD98, 2px -1px 0 #EFCD98,-2px -1px 0 #EFCD98; font-size:7em; text-align: center; width:820px;}
.phb#p1 {background-image: url('https://www.gmbinder.com/images/Nrkf77U.jpg'); background-size: 822px;} /* Fix for image-less covers */

/* Page Numbers */ 
.phb:after { background-image:url('https://www.gmbinder.com/images/O3hOuX8.png?1') !important; background-size: 100px; background-repeat:no-repeat; z-index:-1; margin-bottom: 5px; margin-left: -25px; } /* Styles the box used by page number */
.phb:nth-child(odd):after { transform: rotate(180deg); margin-bottom: 21px; margin-left: 25px; }
.pageNumber.auto { font-family: 'Tauri', sans-serif; color:#58180D; font-size:2em; border-color:#EFCD98; border 10px; text-shadow: 1px 1px 0 #EFCD98, -1px 1px 0 #EFCD98, 1px -1px 0 #EFCD98, -1px -1px 0 #EFCD98, 0px 1px 0 #EFCD98, 0px -1px 0 #EFCD98, -1px 0px 0 #EFCD98, 1px 0px 0 #EFCD98, 2px 2px 0 #EFCD98, -2px 2px 0 #EFCD98, 2px -2px 0 #EFCD98, -2px -2px 0 #EFCD98, 0px 2px 0 #EFCD98, 0px -2px 0 #EFCD98, -2px 0px 0 #EFCD98, 2px 0px 0 #EFCD98, 1px 2px 0 #EFCD98, -1px 2px 0 #EFCD98, 1px -2px 0 #EFCD98, -1px -2px 0 #EFCD98, 2px 1px 0 #EFCD98, -2px 1px 0 #EFCD98, 2px -1px 0 #EFCD98,-2px -1px 0 #EFCD98;} /* Styles the automatically generated page number */
.phb#p1 {counter-reset: phb-page-numbers 0;} /* Allows you to start the page count from a value different than 1st page. Change 0 to the value you want to add to the page number on the 1st page */
.phb#p1 .pageNumber.auto { display:none } /* Hides the page number on the cover page. Remove "none" if you don't use a cover page */
.phb#p1:after { display:none } /* Hides the box used by the page number on the cover page. Remove "none" if you don't use a cover page */

/* Headers */
.phb h1, .phb h2 {font-family: 'Eczar', sans-serif;} /* No Taroca, unless you license it yourself */
.phb h1 {text-align: center;font-size: 5em; margin-bottom:30px;}
.phb h2 {color:#02256E;font-size: 2.25em;}
.phb h3, .phb h4, .phb h5 {font-family: 'Tauri', sans-serif;}
.phb h3 {font-family: 'Teko', sans-serif; font-size: 2em; border-bottom:0px}
.phb h4 {color:#000000;border-bottom:1px solid #000000;margin-bottom:0px; text-transform:uppercase; }
.phb h5 { text-transform:uppercase; }
.phb h6 {background-color:#002664; color:#EDE3C8;border-bottom:1px solid #002664;margin-bottom:5px; padding-left:8px; padding-top:5px; padding-bottom:3px;font-size: 1.25em;font-family: 'Tauri', sans-serif; text-transform:uppercase; border-radius: 12px 12px 0px 0px;}

/* Content */
.phb, .phb p, .phb p+p, .phb ul, .phb ol {font-family:'Gelasio', sans-serif; text-align: justify; text-justify: inter-character; line-height:1.4;}
.phb hr+section blockquote{background : white;}
.flavor {font-family: 'DM Serif Text', serif !important; text-align: justify; text-justify: inter-character; font-size: 1.25em; line-height: 1.4; padding-bottom:8px; padding-left:10px; padding-right:10px; }
.subtitle { font-size: 1.4em; color: #5E0000 !important; background-color:transparent !important; margin-top:-30px; margin-bottom:px !important; margin-right:10px !important; margin-left:10px !important; background-image: url('https://www.gmbinder.com/images/5uPOPvf.png'); background-position:bottom; background-repeat:no-repeat; padding-bottom:35px; background-size:800px; }

/* Tables */
.phb table { background-color: #F5EFE0; margin-bottom:0px; }
.phb table th { background-color: #5E0000; color:white; padding-top:4px; }
.phb table tbody tr:nth-child(odd) { background-color: #EDE3C8 }
.phb table tbody, .phb table th { font-family: 'Roboto Condensed', sans-serif;  }
.tablefooter { background-color:#E6D8B0 !important; }

/* Actions */
.label {font-family: 'Tauri', sans-serif; float: right; text-align:right; inline-block; font-size:.4cm; color:black; margin-bottom:-3px; text-transform:uppercase; border: 0px;}

/* Keywords */
.taglist {height:22px; }
.tag {font-family: 'Roboto Condensed', sans-serif; border-color:#DAC68A; border: 1px solid #DAC68A; border-left: 2px solid #DAC68A; border-right: 2px solid #DAC68A; border-radius:2px; background-color:#58180D; color:white; text-align:center; margin-top:2px; margin-right:2px; min-width:30px; float:left; margin-bottom:-5px; padding-left:3px; padding-right:3px; text-transform:uppercase; }
/*Keyword for Rarities */
.uncommon {background-color:#98513D !important;}
.rare {background-color:#002664 !important;}
.unique {background-color:#54166E !important;}
/* Keyword for Creatures */
.align {background-color:#576293 !important;}
.size {background-color:#3B7B59 !important;}

/* Compact Rules */
.rule, .rule p, .rule p+p {font-family: 'Roboto Condensed', sans-serif; line-height:1.4; }
.rule p, .rule p+p { text-indent:1.5em; line-height:1.4; font-size:100%; }
p .oneaction  { margin-top:-0px; margin-bottom:-0px; width:14px; margin-right:-1px; margin-left:-1px; }
p .twoaction { margin-top:-0px; margin-bottom:-0px; height:22px; width:24px; margin-right:-1px; margin-left:-1px; }
p .threeaction { margin-top:0px; margin-bottom:-0px; height:28px; width:32px; margin-right:-1px; margin-left:-1px; }
h5 .oneaction, h4 .oneaction  { margin-top:-10px; margin-bottom:-6px; width:16px; margin-right:-1px; margin-left:-1px; }
h5 .twoaction, h4 .twoaction { margin-top:-10px; margin-bottom:-6px; height:26px; width:28px; margin-right:-1px; margin-left:-1px; }
h5 .threeaction, h4 .threeaction { margin-top:-10px; margin-bottom:-6px; height:34px; width:38px; margin-right:-1px; margin-left:-1px; }
.rule .oneaction  { width:14px; margin-top:-6px; margin-bottom:-6px; margin-right:-1px; margin-left:-1px; }
.rule .twoaction { height:22px; width:24px; margin-top:-6px; margin-bottom:-6px; margin-right:-1px; margin-left:-1px;}
.rule .threeaction { height:28px; width:32px; margin-top:-7px; margin-bottom:-6px; margin-right:-1px; margin-left:-1px; }
.result {font-family: 'Roboto Condensed', sans-serif; padding-left: 1.5em;text-indent:-1.5em;}
.ability {font-family: 'Roboto Condensed', sans-serif; padding-left: 1.5em;text-indent:-1.5em;}
.abilityname { font-weight: bold; }
.r4:before { content: "Critical Success "; font-weight: bold; }
.r3:before { content: "Success "; font-weight: bold; }
.r2:before { content: "Failure "; font-weight: bold; }
.r1:before { content: "Critical Failure "; font-weight: bold; }
/* Boxed Containers */
.box {border-bottom:1px solid #000000; hyphens: manual; hyphens: auto; word-break: break-word; } /* Normal boxes just put a separator line at the bottom */
.reqbox {border-bottom:1px solid #000000;padding-left: 1.5em;text-indent:-1.5em; hyphens: manual; overflow-wrap: break-word; overflow: hidden; } /* Boxes for requirements and prerequisites require the Pathfinder signature identation */ 
.tab {text-indent:1.5em;  }
/* Labels for Feats and Actions */
.prereq:before { content: "Prerequisites "; font-weight: bold; }
.req:before { content: "Requirements "; font-weight: bold; }
.name { font-style:italic; }
.name:before { content: "Name "; font-weight: bold; font-style:normal; }
.name:after { content: "; "; }
.hands:before { content: "Hands "; font-weight: bold; }
.hands:after { content: "; "; }
/*Labels for Spells */
.traditions:before { content: "Traditions "; font-weight: bold; }
.cast:before { content: "Cast "; font-weight: bold; }
.range { float:left; margin-right:20px;  }
.range:before { content: "Range "; font-weight: bold; }
.range:after { content: ";"; }
.targets:before { content: "Targets "; font-weight: bold; }
.area:before { content: "Area "; font-weight: bold; }
.savingthrow:before { content: "Saving Throw "; font-weight: bold; }
.trigger:before { content: "Trigger "; font-weight: bold; }
.trigger:after { content: "; "; }
.duration:before { content: "Duration "; font-weight: bold; }
.heightened:before { content: "Heightened "; font-weight: bold; }
.heightenedp1:before { content: "Heightened (+1) "; font-weight: bold; }
.heightenedp2:before { content: "Heightened (+2) "; font-weight: bold; }
.heightenedp3:before { content: "Heightened (+3) "; font-weight: bold; }
.heightenedp4:before { content: "Heightened (+4) "; font-weight: bold; }
.heightened1:before { content: "Heightened (1st) "; font-weight: bold; }
.heightened2:before { content: "Heightened (2nd) "; font-weight: bold; }
.heightened3:before { content: "Heightened (3rd) "; font-weight: bold; }
.heightened4:before { content: "Heightened (4th) "; font-weight: bold; }
.heightened5:before { content: "Heightened (5th) "; font-weight: bold; }
.heightened6:before { content: "Heightened (6th) "; font-weight: bold; }
.heightened7:before { content: "Heightened (7th) "; font-weight: bold; }
.heightened8:before { content: "Heightened (8th) "; font-weight: bold; }
.heightened9:before { content: "Heightened (9th) "; font-weight: bold; }
.heightened10:before { content: "Heightened (10th) "; font-weight: bold; }
/*Labels for Spells */
.perception:before { content: "Perception "; font-weight: bold; }
.languages:before { content: "Languages "; font-weight: bold; }
.skills:before { content: "Skills "; font-weight: bold; }
.str { float:left; margin-right:19px;  }
.str:before { content: "Str "; font-weight: bold; }
.str:after { content: "; "; }
.dex { float:left; margin-right:19px;  }
.dex:before { content: "Dex "; font-weight: bold; }
.dex:after { content: "; "; }
.con { float:left; margin-right:19px;  }
.con:before { content: "Con "; font-weight: bold; }
.con:after { content: "; "; }
.int { float:left; margin-right:19px;  }
.int:before { content: "Int "; font-weight: bold; }
.int:after { content: "; "; }
.wis { float:left; margin-right:19px;  }
.wis:before { content: "Wis "; font-weight: bold; }
.wis:after { content: "; "; }
.cha:before { content: "Cha "; font-weight: bold; }
.ac { float:left; margin-right:19px;  }
.ac:before { content: "AC "; font-weight: bold; }
.ac:after { content: "; "; }
.fort { float:left; margin-right:19px;  }
.fort:before { content: "Fort "; font-weight: bold; }
.fort:after { content: "; "; }
.ref { float:left; margin-right:19px;  }
.ref:before { content: "Ref "; font-weight: bold; }
.ref:after { content: "; "; }
.will:before { content: "Will "; font-weight: bold; }
.hp:before { content: "HP "; font-weight: bold; }
.hp:after { content: "; "; }
.bt:before { content: "BT "; font-weight: bold; }
.bt:after { content: "; "; }
.hardness:before { content: "Hardness "; font-weight: bold; }
.hardness:after { content: "; "; }
.immunities:before { content: "Immunities "; font-weight: bold; }
.immunities:after { content: "; "; }
.weaknesses:before { content: "Weaknesses "; font-weight: bold; }
.weaknesses:after { content: "; "; }
.resistances:before { content: "Resistances "; font-weight: bold; }
.speed { clear:left; }
.speed:before { content: "Speed "; font-weight: bold; }
.melee:before { content: "Melee "; font-weight: bold; }
.melee:after { content: ", "; }
.ranged:before { content: "Ranged "; font-weight: bold; }
.ranged:after { content: ", "; }
.damage { word-break: break-all; }
.damage:before { content: "Damage "; font-weight: bold; }
.innatespells { font-weight: bold; }
.innatespells:after { content: " Innate Spells ";  font-weight: bold; }
.preparedspells { font-weight: bold; }
.preparedspells:after { content: " Prepared Spells ";  font-weight: bold; }
.dc:before { content: "DC ";  }
.dc:after { content: ", ";  }
.spellattack:before { content: "attack ";  }
.spellattack:after { content: "; ";  }
.sp1, .sp2, .sp3, .sp4, .sp5, .sp6, .sp7, .sp8, .sp9, .sp10, .can1, .can2, .can3, .can4, .can5, .can6, .can7, .can8, .can9, .can10 { font-style: italic; }
.sp1:before { content: " 1st "; font-weight: bold; font-style: normal; }
.sp2:before { content: " 2nd "; font-weight: bold; font-style: normal; }
.sp3:before { content: " 3rd "; font-weight: bold; font-style: normal; }
.sp4:before { content: " 4th "; font-weight: bold; font-style: normal; }
.sp5:before { content: " 5th "; font-weight: bold; font-style: normal; }
.sp6:before { content: " 6th "; font-weight: bold; font-style: normal; }
.sp7:before { content: " 7th "; font-weight: bold; font-style: normal; }
.sp8:before { content: " 8th "; font-weight: bold; font-style: normal; }
.sp9:before { content: " 9th "; font-weight: bold; font-style: normal; }
.sp10:before { content: " 10th "; font-weight: bold; font-style: normal; }
.can1:before { content: " Cantrips (1st) "; font-weight: bold; font-style: normal; }
.can2:before { content: " Cantrips (2nd) "; font-weight: bold; font-style: normal; }
.can3:before { content: " Cantrips (3rd) "; font-weight: bold; font-style: normal; }
.can4:before { content: " Cantrips (4th) "; font-weight: bold; font-style: normal; }
.can5:before { content: " Cantrips (5th) "; font-weight: bold; font-style: normal; }
.can6:before { content: " Cantrips (6th) "; font-weight: bold; font-style: normal; }
.can7:before { content: " Cantrips (7th) "; font-weight: bold; font-style: normal; }
.can8:before { content: " Cantrips (8th) "; font-weight: bold; font-style: normal; }
.can9:before { content: " Cantrips (9th) "; font-weight: bold; font-style: normal; }
.can10:before { content: " Cantrips (10th) "; font-weight: bold; font-style: normal; }
/* Labels for Hazards */
.stealth:before { content: "Stealth "; font-weight: bold; }
.description:before { content: "Description "; font-weight: bold; }
.disable:before { content: "Disable "; font-weight: bold; }
.routine:before { content: "Routine "; font-weight: bold; }
.reset:before { content: "Reset "; font-weight: bold; }
/* Labels for Items */
.price:before { content: "Price "; font-weight: bold; }
.usage:before { content: "Usage "; font-weight: bold; }
.usage:after { content: "; ";  }
.bulk:before { content: "Bulk "; font-weight: bold; }
.bulk:after { content: "; ";  }
.type { font-style:italic; }
.type:before { content: "Type "; font-weight: bold; font-style:normal; }
.level:before { content: "Level "; font-weight: bold; }
.activate:before { content: "Activate "; font-weight: bold; }
.activate:after { content: "; ";  }
.effect:before { content: "Effect "; font-weight: bold; }
.onset:before { content: "Onset "; font-weight: bold; }
.maxduration:before { content: "Maximum Duration "; font-weight: bold; }
.stage1:before { content: "Stage 1 "; font-weight: bold; }
.stage2:before { content: "Stage 2 "; font-weight: bold; }
.stage3:before { content: "Stage 3 "; font-weight: bold; }
.stage4:before { content: "Stage 4 "; font-weight: bold; }
.stage5:before { content: "Stage 5 "; font-weight: bold; }
.stage6:before { content: "Stage 6 "; font-weight: bold; }
.craftrequirements:before { content: "Craft Requirements "; font-weight: bold; }
.savingthrow:after, .onset:after, .maxduration:after, .stage1:after, .stage2:after, .stage3:after, .stage4:after, .stage5:after, .stage6:after, .level:after, .type:after { content: "; "; }
.quantity:before { content: "Quantity "; font-weight: bold; }
.quantity:after { content: "; "; }
.ammunition:before { content: "Ammunition "; font-weight: bold; }
.special:before { content: "Special "; font-weight: bold; }
.sageadvice:before { content: "Developer Feedback "; font-weight: bold; }
.damage:before { content: "Damage "; font-weight: bold; }
.damage:after { content: "; ";  }
.thrown:before { content: "thrown "; font-weight: bold; }
.criticalspecialization:before { content: "Critical Specialization "; font-weight: bold; }

/* Sidebar */
.smallsidebar { background-image: url("https://pf2.easytool.es/sheets/boxBorder2.png"); background-size: 350px; background-repeat:no-repeat; margin-left:-1em; margin-right:-3em; padding-left:2.6em; padding-right:3em; padding-top:2.5em; display:inline-block; padding-bottom:40px; }
.smallsidebar h5 { text-align:center; padding-bottom:10px; text-transform:uppercase; }
.smallsidebar p, .smallsidebar p+p { background-color: #DBD1BC; font-family: 'Roboto Condensed', sans-serif; margin-left:-10px; padding-left:13px; margin-right:-8px; padding-right:12px; width:309px; margin-top:-11px; }

/* Dual Sidebar */
.dualsidebar { background-image: url("https://www.gmbinder.com/images/M2t21DV.png"), url("https://www.gmbinder.com/images/sVseLe2.png"); background-position: -10% 100%, top left; background-size: 705px,705px; background-repeat:no-repeat; margin-left:0.7em; padding-left:1.75em; padding-right:3.5em; padding-top:3.2em; padding-bottom:40px; margin-right:-35px;}
.phb:nth-child(odd) .dualsidebar { margin-left:-25px !important; margin-right:0px; padding-left:3.5em; padding-right:2em; } /* This code moves tables 35px right on odd pages, avoiding the table overlapping the page's image margin */
.dualsidebar h5 { text-align:center; background-color: #C4B8A0; margin-left:px; margin-right:px; padding-bottom: 8px; margin-top:5px; margin-bottom:-2px; }
.dualsidebar p, .dualsidebar p+p { background-color: #C4B8A0; font-family: 'Roboto Condensed', sans-serif; margin-left:-17px; padding-left:13px; margin-right:-15px; padding-right:12px; }

/* Red Sidebar */
.redsidebar { border-image-slice:35 41 37 41 fill;border-image-width:60px 60px 60px 60px;border-image-outset:0px 0px 0px 0px;border-image-repeat:stretch stretch;border-image-source:url("https://www.gmbinder.com/images/Gl8LTE9.png"); border-top:32px solid; border-bottom: 32 solid; margin-left:-3em; margin-right:-3em; padding-left:2.6em; padding-right:3em; padding-top:1.5em; padding-bottom:40px;}
.redsidebar h2 { font-family: 'Eczar', sans-serif; text-align:center; color:#CFBF80; background-color: #5E0000; margin-left:-px; margin-right:-8px; padding-bottom: 8px; margin-top:-5px; margin-bottom:-2px; font-size:1.5em; }
.redsidebar h3 { font-family: 'Eczar', sans-serif; text-align:center; color:WHITE; background-color: #5E0000; margin-left:-px; margin-right:-8px; padding-bottom: 8px; margin-top:-5px; margin-bottom:-2px; font-size:2em; }
.redsidebar h3 span { text-align:left; }
.redsidebar img { height: 450px; margin-top:-30px; align:right; display: block; margin-left: auto; margin-right: auto; }
.redsidebar h5 { text-align:left; color:white; background-color: #5E0000; margin-left:-px; margin-right:-8px; padding-bottom: 8px; margin-top:7px; margin-bottom:-2px; }
.redsidebar p, .redsidebar p+p, .redsidebar .flavor, .dualredsidebar .flavor { background-color: #5E0000; color:white; font-family: 'Roboto Condensed', sans-serif; margin-left:-13px; padding-left:13px; margin-right:-8px; padding-right:-12px; }
.redseparatorfull { background-image: url("https://www.gmbinder.com/images/gRfVwlG.png"); background-size:390px; height:35px; margin-right:-20px; margin-left:-14px; margin-top:-6px; }
.redseparatorsmall { background-image: url("https://www.gmbinder.com/images/LlbSin0.png"); background-size:375px; background-position:top center; height:4px; margin-bottom:5px; margin-top:-5px;  margin-right:-20px; margin-left:-14px; }
.redsidebar .toc { background-image: url("https://www.gmbinder.com/images/Lw65fTb.png"), url("https://www.gmbinder.com/images/kCLyCck.png"); background-position: bottom right, top; background-size: 392px,392px; background-repeat:no-repeat;  }

/* Dual Red Sidebar */
.dualredsidebar { background-image: url("https://www.gmbinder.com/images/JwtgIpO.png"), url("https://www.gmbinder.com/images/SXJd6Hg.png"); background-position: bottom left, top left; background-size: 705px,705px; background-repeat:no-repeat; margin-left:0.7em; margin-right:-3em; padding-left:2.6em; padding-right:3em; padding-top:3.2em; padding-bottom:30px;}
.dualredsidebar h5 { text-align:center; color:white; background-color: #5E0000; margin-left:px; margin-right:px; padding-bottom: 8px; margin-top:5px; margin-bottom:-2px; }
.dualredsidebar p, .dualredsidebar p+p { background-color: #5E0000; color:white; font-family: 'Roboto Condensed', sans-serif; margin-left:-9px; padding-left:0px; margin-right:-6px; padding-right:12px; }
.phb:nth-child(odd) .dualredsidebar { margin-left:-25px !important; margin-right:-21px; padding-left:45px;} /* This code moves tables 35px right on odd pages, avoiding the table overlapping the page's image margin */
.dualredsidebar .flavor, .dualredsidebar h5 { margin-left:-15px !important; margin-right:15px !important; }

/* Wide Page Sidebar */
.widepage {display: grid; grid-template-columns: 530px 250px; } /* Creates a grid with two columns with variable width. The sidebar column is on the right. */
.phb:nth-child(odd) .widepage {margin-left:-30px; } /* Moves the wide page grid to the right on odd pages */
.widepageright {display: grid; grid-template-columns: 250px 530px; } /* Creates a grid with two columns with variable width. The sidebar column is on the left. */
.phb:nth-child(odd) .widepageright {margin-left:-30px; }  /* Moves the wide page grid to the right on odd pages */
.widebar { }
.thinbar { color:#5E0004; font-size: 0.9em; margin-top:0px; margin-left:10px; padding-left:10px; margin-right:65px; border-left: 1px solid #5E0004; }
.widebarright { margin-left:-50px; margin-right:60px; }
.thinbarright { color:#5E0004; font-size: 0.9em; margin-top:0px; margin-right:10px; padding-right:10px; margin-right:65px; border-right: 1px solid #5E0004; }
.thinbar h3, .thinbarright h3 { font-size:2em;font-weight: normal; } /* Sidebars use a smaller heading 3, so bold weight needs to be removed */
.thinbar p, .thinbar p+p, .thinbar ul, .thinbar ol { font-family: 'Roboto Condensed', sans-serif;  }

/* table of contents */
.toc { padding-left:40px;padding-right:45px; margin-left:-37px; }
.toc a {
 color: #F2EFEA !important;	/*toc specifically wants black text. This resets the headers*/}
.toc li span:nth-child(2){ /*Allow dot leaders to fill remaining space but not overlap*/
 width: auto;
 overflow: hidden;
 white-space: nowrap; 
 display: block; 
 font-family: 'Roboto Condensed', sans-serif;}
.toc li span:nth-child(2):after{
 font-family: 'Roboto Condensed', sans-serif;
 font-size: 0.317cm;
 font-weight: normal;
 color: #F2EFEA;
 content:" ........................................" "........................................." ".........................................";}
.toc li span:first-child{ /*Remove any header styles from page numbers*/
 float: right;
 font-family: 'Roboto Condensed', sans-serif;
 font-size: 0.317cm;
 font-weight: normal;
 color: #F2EFEA;
 margin-left: 1px; /*Leaves a small space between page numbers and dot leaders*/}
/*Special cases for headings*/    
.toc li h3 span:nth-child(2):after{content: " ";/*Remove dot leaders on h3*/}
.toc li h3 {
 margin-bottom: 4px !important;	/*Special spacing for h3*/
 margin-top: 10px !important;
 line-height: initial !important; /*For some reason Multi-line h3 line spacing changed*/}
.toc li h3 span:first-child{line-height: 1.8em !important; /*Line page numbers up with Multi-line h3 better*/}
.toc ul ul {margin-left: 10px !important; font-size: 0.375cm; /*Original lists intented too much*/}
.toc>ul>li {margin-bottom: initial !important; /*margin for list items needs to be removed or 0*/}

/* Fixes */   
.phb:after { content: ""; } /*  Removes Wizards of the Coast disclaimer. I should probably add OGL disclaimer. */
.phb {padding-bottom:0.5cm;} /* Minimizes the bottom padding of pages so that less content spills across columns */
.dualsidebarfix { margin-left:-65px; margin-right:75px; margin-top:-40px; padding-bottom:40px; } /* Dual Sidebars needs repositioning of two column content */
.phb#p1 { padding-left: 0px; padding-right:0px; } /* Remove this if you do not use a cover */
.phb:nth-child(even) { padding-left: 75px; padding-right:1.5cm }
.phb:nth-child(odd) { padding-left: 55px; padding-right:75px; }

/* Paizo Compatibility Fixes */   
/* .pathfinderlogo { display:none; } */
/* .secondedition { display:none; } */
.bookcover { display:none; }
/* .phb#p1, .phb, .phb:nth-child(odd) {background-image: none; background-color:#EFECE7;} */
/* .phb:after { display:none; } */
/* The following lines remove the Page Margin Bauble completely */
.p.hb { background-image: url('https://www.gmbinder.com/images/sPk1xm4.png'), url('https://www.gmbinder.com/images/EABESdy.png'); } 
.p.hb:nth-child(odd) { background-image: url('https://www.gmbinder.com/images/4PiRxoX.png'), url('https://www.gmbinder.com/images/EABESdy.png'); }
/* The following lines put a non-Paizo Dragon in the Page Margin Bauble */
.phb { background-image: url('https://www.gmbinder.com/images/REmFBe1.png'), url('https://www.gmbinder.com/images/EABESdy.png'); } 
.phb:nth-child(odd) { background-image: url('https://www.gmbinder.com/images/IQwl0gO.png'), url('https://www.gmbinder.com/images/EABESdy.png'); }
.amiri { opacity: 0.0; }

</style>

<img src='https://www.gmbinder.com/images/c3QzBcJ.png' class='cover-image bookcover'>

<div class='cover-title' style='margin-top:780px; '>Your Title Here</div>

<img src='https://www.gmbinder.com/images/NUdbnd3.png' class='pathfinderlogo cover-image' style="width:80%;margin-left:90px;margin-top:30px">

<img src='https://www.gmbinder.com/images/4wBBdP2.png' class='covertitle cover-image' style="width:35%;margin-left:520px;margin-top:970px">

<img src='https://www.gmbinder.com/images/7JHDdb0.png' class='secondedition cover-image' style="width:35%;margin-left:532px;margin-top:0px">

<div class='secondedition cover-header' style="font-family: 'Eczar', sans-serif; margin-top:-32px; margin-left:-240px; color:#5E0000; border:0px; font-size: 1.1em; text-shadow: 0px 0px 0px; text-align:right; ">SECOND EDITION</div>

\pagebreakNum



<div style="text-align:center; margin-top:50px;">

## Pathfinder 2nd Edition needs your homebrew!

</div>

This template allows you to create professional-looking homebrew documents for the *Pathfinder Second Edition* that will impress online communities and your players. While not a pixel-perfect carbon copy of the complex typography used by Paizo, this template attempts to faithfully reproduce every aspect of the layout, and will be regularly updated with new visual elements as they are introduced in later books.

### Copyrighted Content

All artwork and visual layout elements in this template are copyrighted by Paizo Inc. and are used for demonstration purposes only. If you plan to distribute homebrew material using this template you must remove all elements that are copyrighted: page border, parchment background and the sidebar backgrounds. However, you may use this template to share homebrew with your players, as is.

**Cover:** *"Pathfinder Roleplaying Game"* by David Alvarez is licensed under **CC BY-NC 4.0**.

### Fonts Used

Paizo uses multiple commercial fonts for their signature **Corebook** layout. I have been able to find fitting equivalents available for non-commercial use via Google Web Fonts.

The only exception is the font **Taroca** used in Pathfinder Corebook for book name and chapter and section titles. This font has unique design and is without alternative. It can be licensed from [Monotype](https://www.myfonts.com/fonts/bluevinyl/taroca/) as Web Font. It costs $28.00 and allows you 10,000 page views per month, more than enough if you do not share the GMBinder link but instead use it only to print PDFs. To implement it, add the @import code in the template style, then change all references to *Eczar* font with *Taroca Regular*.

### Get Support

This template is created and maintained by Apostol Apostolov. You can find me on [Reddit](https://www.reddit.com/user/theapoapostolov), or the [Grit and Glory Discord](https://discord.gg/ZDtCmhm).

<center><a href="https://discord.gg/ZDtCmhm"><img src="https://www.gmbinder.com/images/4aNOoiD.png" style="width:180px;"></a></center><br>

### Changelog

#### V1.041 – 7th of March 2020
**This is the first public release of the template.** Improved HTML format of the item and creature templates. Fixed printing margins required by latest versions of the Chrome browser. Fixed sizes and templates for action icons.

\columnbreak

<div class="redsidebar toc">

## TABLE OF CONTENTS

<div class="flavor">Use this column to create a table of contents so readers navigate through your rulebook with a click. The page number or range of pages must be put in the SPAN and also in the hyperlink field at the end of each entry. When printed to a PDF, these links will still work.</div>

<div class="flavor">An alternative method of maintaining Table of Contents entries is to check the raw HTML of the document for the exact naming of section tags. By using section tags instead of pages, the entries will update as your content is pushed to a new page.</div>
 
- ### [<span></span><span>Chapter One</span>](#p3)
  - [<span>4</span><span>Section One</span>](#p4)
  - [<span>5</span><span>Section Two</span>](#p5)
  - [<span>6</span><span>Section Three</span>](#p6)
- ### [<span></span><span>Chapter Two</span>](#p7)
  - [<span>8</span><span>Section One</span>](#p8)
  - [<span>9</span><span>Section Two</span>](#p9)
  - [<span>10</span><span>Section Three</span>](#p10)
- ### [<span></span><span>Chapter Three</span>](#p11)
  - [<span>12</span><span>Section One</span>](#p12)
  - [<span>13</span><span>Section Two</span>](#p13)
  - [<span>14</span><span>Section Three</span>](#p14)  
 

<div style="height:280px;"></div>

</div>


\pagebreakNum

# Chapter Title (#)

<div class="wide flavor subtitle">This is a "wide" one column text, using "flavor" serif font used for lore and flavor text and "sibtitle" for displaying flavor under a chapter title. Even if you have no subtitle, this div is needed to display the fancy separator line under the chapter title. </div>

## Header 2 (##)

Use this header for subchapters, such as different types of equipment in the Equipment chapter. 

### Header 3 (###)

Use this header for various topics and separate rules, such as different aspects of combat.  

#### Header 4 (####)

Use this header for feats and actions that need a separating line from the content below it.

##### Header 5  (#####)

Use this header for feats, actions and similar items that do not need a separating line from the content below it.

###### Header 6 (######)

Use this header for separating feats for specific level from those requiring lower or higher level. 

## Action Icons

The action icons supported are: {0A} {1A} {2A} {3A} {R} {P}

Instead adding image code every time you want to use icons, this template uses the GMBinder variables. They are already configured for you so all you need is use the codes 0A (free action), 1A (one action), 2A (two actions), 3A (three actions), R (reaction) and P (passive action). You can add more icons as they are introduced in Pathfinder rules using similar HTML code (and image should be hosted on Imgur).

<img src="https://www.gmbinder.com/images/MLzFjmc.png" width=330>

\columnbreak

## Example Feat 

#### Feat Title {1A} <div class="label">FEAT 1</div>
<div class="taglist">
<div class="tag uncommon">UNCOMMON</div>
<div class="tag rare">RARE</div>
<div class="tag unique">UNIQUE</div>
<div class="tag">KEYWORD</div>
</div>
<div class="reqbox">
<div class="rule prereq">List prerequisites such as skill proficiency here.</div>
<div class="rule req">List requirements such as items held here.</div>
</div>
<div class="rule">
Write the rules of the feat or action here, without including the results (such as success or failure) of the action. They use the HTML code blocks below. Do not add "Sucess" or "Failure" before the results as these words are added automatically, in bold. Markdown code can't be used in rule texts using this font.

<div class="rule result r4">Critical Success result is written here. As you can see the results support Pathfinder's signature indentation.</div>
<div class="rule result r3">Success result is written here.</div>
<div class="rule result r2">Failure result is written here.</div>
<div class="rule result r1">Critical failure result is written here.</div>
</div><br>

## Example Action

#### Action Title {2A} {2A} {3A} 
<div class="taglist">
<div class="tag uncommon">UNCOMMON</div>
<div class="tag rare">RARE</div>
<div class="tag unique">UNIQUE</div>
<div class="tag">KEYWORD</div>
</div>
<div class="rule">You spend 10 minutes to do a specific action and one of several results may occur. </div>
<div class="rule result r4">Critical Success result is written here. As you can see the results support Pathfinder's signature indentation.</div>
<div class="rule result r3">Success result is written here.</div>
<div class="rule result r2">Failure result is written here.</div>
<div class="rule result r1">Critical failure result is written here.</div><br>

## Example Spell

#### Spell Title <div class="label">SPELL 1</div>
<div class="taglist">
<div class="tag uncommon">UNCOMMON</div>
<div class="tag rare">RARE</div>
<div class="tag unique">UNIQUE</div>
<div class="tag">KEYWORD</div>
</div>
<div class="reqbox"><div>
<span class="rule traditions">arcane, divine, occult, primal</span>
</div><div>
<span class="rule cast">{2A} somatic, verbal</span>
</div><div>
<span class="rule trigger">Needed for reaction spells.<</span>
</div><div>
<span class="rule range">touch</span><span class="rule targets">any number of creatures</span>
</div><div>
<span class="rule area">20-foot burst</span>
</div><div>
<span class="rule savingthrow">Fortitude, Reflex or Will</span>
</div></div>
<div class="box">
<div class="rule">Add the spell effect here. You can copy result effects (r1 to r4 styles) from the above examples. Remember, you can't bold or italic using Markdown in <i>rule</i> fields. </div>
</div>
<div class="rule heightenedp1">The spell has improved effect.</div>
<div class="rule heightened3">Check the CSS for all heightened options.</div>

\pagebreakNum


## Example Creature

Use Heading 2 for creature families that may contain one or several creatures with similar traits and abilities. 

### Creature Name

Use Heading 3 for individual creatures and their description, lore, habitat and behavior. 

#### Creature Name <div class="label">CREATURE 1</div>
<div class="taglist">
<div class="tag uncommon">UNCOMMON</div>
<div class="tag rare">RARE</div>
<div class="tag unique">UNIQUE</div>
<div class="tag align">LE</div>
<div class="tag size">MEDIUM</div>
<div class="tag">KEYWORD</div>
</div>
<div class="reqbox">
<div>
<span class="rule perception">+5; darkvision</span>
</div><div>
<span class="rule languages">common</span>
</div><div>
<span class="rule skills">Acrobatics +12, Diplomacy +15, Intimidating +12, Performance +17, Religion +14</span></div>
<div>
<span class="rule str">+1</span>
<span class="rule dex">+2</span>
<span class="rule con">+3</span>
<span class="rule int">+0</span>
<span class="rule wis">-5</span>
<span class="rule cha">+2</span>
</div>
</div><div class="reqbox">
<div>
<span class="rule ac">19 (14 when broken)</span>
<span class="rule fort">+3</span>
<span class="rule ref">+6</span>
<span class="rule will">+3</span>
</div>
<div>
<span class="rule hp">48</span>
<span class="rule hardness">8</span>
<span class="rule immunities">bleed, death effects, disease, doomed, drained, fatigued, healing, mental, necromancy, nonlethal attacks, paralyzed, poison, sickened, unconscious</span>
<span class="rule weaknesses">cold 10</span>
<span class="rule resistances">fire 5</span>
</div></div><div class="reqbox">
<div>
<span class="rule speed">30 feet</span>
</div><div>
<span class="rule melee">{1A}  stone fist +19 (magical) </span>
<span class="rule damage"> 2d12+6 bludgeoning plus Grab</span>
</div><div>
<span class="rule ranged">{1A} flaming coal +12 (finesse, fire, magical, range increment 80 feet)</span>
<span class="rule damage">2d6+6 bludgeoning and 2d8 fire</span>
</div><div>
<span class="rule innatespells">Arcane</span>
<span class="rule dc">23</span>
<span class="rule spellattack">+14</span>
<span class="rule sp2"> dispel magic, invisibility, resist energy</span>
<span class="rule sp1">ray of enfeeblement, true strike (×2);</span>
<span class="rule can2">detect magic, ghost sound, mage hand, ray of frost, read aura</span>
</div><div class="rule">
<span class="abilityname">Ability Name</span> 
<span class="rule">{2A} Describe your ability here and set the proper action icon. You can copy paragraphs like this one in any section above to explain an innate ability or reaction of the creature.</span>
</div></div>

<br>

## Example Hazard

#### Hazard Name <div class="label">Hazard 1</div>
<div class="taglist">
<div class="tag uncommon">UNCOMMON</div>
<div class="tag rare">RARE</div>
<div class="tag unique">UNIQUE</div>
<div class="tag">KEYWORD</div>
</div><div class="reqbox"><div>
<span class="rule stealth">+20</span>
</div><div>
<span class="rule description">Describe what the hazard looks like.</span>
</div></div>
<div class="reqbox"><div>
<span class="rule disable">Acrobatics DC 13 to approach without triggering the trap followed by Thievery DC 15 (trained) to disable it. </span>
</div><div>
<span class="rule ac">23</span>
<span class="rule fort">+13</span>
<span class="rule ref">+6</span>
<span class="rule will">+3</span>
</div><div>
<span class="rule abilityname">Hazard Action</span> Define each of the actions of the hazard.</span>
</div><div>
<span class="rule routine">Long description of the behavior model of a complex hazard.</span>
</div></div><div><div>
<span class="rule reset">Conditions that must be met for the hazard to reset. </span>
</div>
</div>

\columnbreak

## Example Item

#### Item Name <div class="label">ITEM 1</div>
<div class="taglist">
<div class="tag uncommon">UNCOMMON</div>
<div class="tag rare">RARE</div>
<div class="tag unique">UNIQUE</div>
<div class="tag">KEYWORD</div>
</div>
<div class="reqbox"><div>
<span class="rule price">10 gp</span>
</div><div>
<span class="rule usage">held with 2 hands</span>
<span class="rule bulk">L</span>
</div><div>
<span class="rule activate">{2A} interact</span>
</div></div>
<div class="box"><div>
<span class="rule hardness">4</span>
<span class="rule hp">16</span>
<span class="rule bt">8</span>
</div><div>
<span class="rule">Description of the item. If it is a poison, apply the block below. Remove it the item is not a poison.</span>
</div><div class="tab">
<span class="rule savingthrow">DC 40 Fortitude</span>
<span class="rule onset">30 minutes</span>
<span class="rule maxduration">1 day</span>
<span class="rule stage1">1d6 poison damage and enfeebled 1 (10 minutes)</span>
<span class="rule stage2">2d6 poison damage and enfeebled 1 (10 minutes)</span>
<span class="rule stage3">2d6 poison damage and enfeebled 1 (10 minutes)</span>
<span class="rule stage4">2d6 poison damage and enfeebled 1 (10 minutes)</span>
<span class="rule stage5">2d6 poison damage and enfeebled 1 (10 minutes)</span>
<span class="rule stage6">2d6 poison damage and enfeebled 1 (10 minutes)</span>
</div></div>
<div class="box"><div>
<span class="rule type">lesser</span>
<span class="rule level">1</span>
<span class="rule price">10 gp</span>
</div><div>
<span class="rule">This item has +1 item bonus.</span>
</div></div>
<div class="box"><div>
<span class="rule type">greater</span>
<span class="rule level">6</span>
<span class="rule price">160 gp</span>
</div><div>
<span class="rule">This item has +2 item bonus.</span>
</div></div>
<div class=""><div>
<span class="rule type">major</span>
<span class="rule level">12</span>
<span class="rule price">960 gp</span>
</div><div>
<span class="rule">This item has +3 item bonus.</span>
</div></div>

<div style="height:30px"></div>

<div class="smallsidebar">

##### CREATING NEW TEMPLATES

If you check the HTML code and CSS classes for each entry, you will quickly understand how to modify and create your own templates. By using predefined properties , that insert their name (in bold) using the :before property and separate with semicolon with the :after property, this saves you time when copying templates or starting new ones from scratch. 

If you must have multiple properties on a single line, create a DIV container and place each property using a SPAN tag. This will ensure that each property follows the previous one, with the constraint of the DIV container. 

One or several properties are placed in a single container that puts a bottom separator line between its content and the next container. These containers use the classes <i>box</i> and <i>reqbox</i>. The difference between them is that reqbox forces the Pathfinder signature identation while <i>box</i> doesn't. Also, if you need to force standard identation, use the <i>tab</i> class (see poison properties of the example item). <br><br>

</div>

\pagebreakNum

# Tables and Sidebars

<div class="wide flavor subtitle"></div>

##### Table 1-1: One Column Table

| Header 1  | Header 2 |
|:---:|:-----------:|
|  1  | One |
|  2  | Two |
|  3  | Three |
|  4  | Four |

<div class="tablefooter rule">* This is a table footer clarification used to expand on table content. </div>

##### Table 1-2: Two Column Table

<div style='column-count:2; column-gap:1px; column-rule: 2px solid #5E0000; ' >

| Header 1  | Header 2 |
|:---:|:-----------:|
|  1  | One |
|  2  | Two |
|  3  | Three |
|  4  | Four |

| Header 1  | Header 2 |
|:---:|:-----------:|
|  5  | Five |
|  6  | Six |
|  7  | Seven |
|  8  | Eight |

</div>

<div class="tablefooter rule">* You can expand, even if the table has multiple columns. </div>

<div class="tablefooter"></div>

<br>

## Sidebars

<div class="smallsidebar">

##### SMALL SEPIA SIDEBAR

This sidebar is usually reserved for small amount of related content, such as rule clarifications, rule examples, check examples related to different levels of skill proficiency, etc.

The contents of this sidebar is made of a title image and the rest of the text has a matching color background that extends as far as you push the content of this sidebar. Still, don't use it for one-line content as some of the background may spill out. 

I still haven't figured how to add bottom padding to this sidebar so meanwhile use dual breaks < br > < br > <br><br>

</div>

\columnbreak

<div class="redsidebar">

## SAMPLE CHARACTER

<div class="redseparatorfull"></div>

<div class="amiri"><img src="https://www.gmbinder.com/images/KWt2cAx.png" style="height:410px;" ></div>

### CHARACTER NAME

<div class="flavor">Some fitting character flavor. </div>

<div class="redseparatorfull"></div>

##### ABILITY SCORES
Write archetype's suggested ability score improvements.

<div class="redseparatorsmall"></div>

##### SKILLS
Write archetype's suggested skill choices here. 

<div class="redseparatorsmall"></div>

##### FEATS
Write archetype's suggested feat advancements here. 

<div class="redseparatorsmall"></div>

##### AND MORE...
You can use the red column sidebar for any type of content that is longer than 1/3 of a column. Great for longer rule clarifications or optional rules, or any content that needs to draw reader attention.

<div class="redseparatorsmall"></div>

</div>

\pagebreakNum

<div class="dualsidebar wide">

##### MULTIPLE COLUMN SEPIA PAGEBOX

<div class="wide flavor">When a sidebar is not enough you can fit half a page of rules in the Pagebox format.</div>

<div class="dualsidebarfix" style="column-count:1;">

#### TABLE 2-1: CLASS SPELLS BY LEVEL
| Your<br>Level | Cantrips | 1st | 2nd | 3rd | 4th | 5th | 6th | 7th | 8th | 9th | 10th
|:---:|:---:|:---|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|1|5|2|—|—|—|—|—|—|—|—|—
|2|5|3|—|—|—|—|—|—|—|—|—
|3|5|3|2|—|—|—|—|—|—|—|—
|4|5|3|3|—|—|—|—|—|—|—|—
|5|5|3|3|2|—|—|—|—|—|—|—
|6|5|3|3|3|—|—|—|—|—|—|—
|7|5|3|3|3|2|—|—|—|—|—|—
|8|5|3|3|3|3|—|—|—|—|—|—
|9|5|3|3|3|3|2|—|—|—|—|—
|10|5|3|3|3|3|3|—|—|—|—|—
|11|5|3|3|3|3|3|2|—|—|—|—
|12|5|3|3|3|3|3|3|—|—|—|—
|13|5|3|3|3|3|3|3|2|—|—|—
|14|5|3|3|3|3|3|3|3|—|—|—
|15|5|3|3|3|3|3|3|3|2|—|—
|16|5|3|3|3|3|3|3|3|3|—|—
|17|5|3|3|3|3|3|3|3|3|2|—
|18|5|3|3|3|3|3|3|3|3|3|—
|19|5|3|3|3|3|3|3|3|3|3|1*
|20|5|3|3|3|3|3|3|3|3|3|1*

<div class="tablefooter rule">* This is a table footer clarification used to expand on table content. </div>

</div></div>

<div class="dualredsidebar wide">

##### MULTIPLE COLUMN RED PAGEBOX

<div class="wide flavor">You can use flavor text as wide content in your pageboxes.  </div>

<div class="dualsidebarfix" style="column-count:3;">

You can have one, two, three or as many columns as you want in your pageboxes. Just set the "column-count" value to the number of columns, and use \ columnbreak to separate each column inside the div. 

The multiple content pagebox is not meant for small amount of content and will break the decoration on the corners if you use it for less than 15 lines of text (in at least one of the columns, or the total text). If you have such case it is best that you use the single column sidebars, not a pagebox. 

You can have one, two, three or as many columns as you want in your pageboxes. Just set the "column-count" value to the number of columns, and use \ columnbreak to separate each column inside the div. 

The multiple content pagebox is not meant for small amount of content and will break the decoration on the corners if you use it for less than 15 lines of text (in at least one of the columns, or the total text). If you have such case it is best that you use the single column sidebars, not a pagebox. 

You can have one, two, three or as many columns as you want in your pageboxes. Just set the "column-count" value to the number of columns, and use \ columnbreak to separate each column inside the div. 

The multiple content pagebox is not meant for small amount of content and will break the decoration on the corners if you use it for less than 15 lines of text (in at least one of the columns, or the total text). If you have such case it is best that you use the single column sidebars, not a pagebox.

</div></div>

\pagebreakNum

# Wide Page Format

<div class="wide flavor subtitle">Pathfinder chapters, such as new classes, usually start with a wide column format with a small sidebar. Bestiary uses this format almost completely.</div>

<div class='wide widepage'> 

<div class="widebar">

## Some Lorem Ipsum...

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

</div>

<div class="thinbar rule">

### Your Sidebar

You can fit all kind of content in the sidebar, such as rule clarifications, optional rules, starting proficiencies for classes, tidbits of lore and anything else. 

</div></div>

<br><br><br><br><br><br>

<div class="wide flavor subtitle">It is up to you to choose between sidebar on the right or on the left. On odd pages the content of the wide page will be shifted so that it doesn't overlap the edge of the page.</div>

<div class='wide widepageright'> 

<div class="thinbarright rule">

### Your Sidebar

You can fit all kind of content in the sidebar, such as rule clarifications, optional rules, starting proficiencies for classes, tidbits of lore and anything else. 

</div>

<div class="widebarright">

## Some Lorem Ipsum...

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

</div></div>

\pagebreakNum

<div style="font-size:95%;">

### OPEN GAME LICENSE Version 1.0a
The following text is the property of Wizards of the Coast, Inc. and is Copyright 2000 Wizards of the Coast, Inc ("Wizards"). All Rights Reserved.

1. Definitions: (a)"Contributors" means the copyright and/or trademark owners who have contributed Open Game Content; (b)"Derivative Material" means copyrighted material including derivative works and translations (including into other computer languages), potation, modification, correction, addition, extension, upgrade, improvement, compilation, abridgment or other form in which an existing work may be recast, transformed or adapted; (c) "Distribute" means to reproduce, license, rent, lease, sell, broadcast, publicly display, transmit or otherwise distribute; (d)"Open Game Content" means the game mechanic and includes the methods, procedures, processes and routines to the extent such content does not embody the Product Identity and is an enhancement over the prior art and any additional content clearly identified as Open Game Content by the Contributor, and means any work covered by this License, including translations and derivative works under copyright law, but specifically excludes Product Identity. (e) "Product Identity" means product and product line names, logos and identifying marks including trade dress; artifacts; creatures characters; stories, storylines, plots, thematic elements, dialogue, incidents, language, artwork, symbols, designs, depictions, likenesses, formats, poses, concepts, themes and graphic, photographic and other visual or audio representations; names and descriptions of characters, spells, enchantments, personalities, teams, personas, likenesses and special abilities; places, locations, environments, creatures, equipment, magical or supernatural abilities or effects, logos, symbols, or graphic designs; and any other trademark or registered trademark clearly identified as Product identity by the owner of the Product Identity, and which specifically excludes the Open Game Content; (f) "Trademark" means the logos, names, mark, sign, motto, designs that are used by a Contributor to identify itself or its products or the associated products contributed to the Open Game License by the Contributor (g) "Use", "Used" or "Using" means to use, Distribute, copy, edit, format, modify, translate and otherwise create Derivative Material of Open Game Content. (h) "You" or "Your" means the licensee in terms of this agreement.

2. The License: This License applies to any Open Game Content that contains a notice indicating that the Open Game Content may only be Used under and in terms of this License. You must affix such a notice to any Open Game Content that you Use. No terms may be added to or subtracted from this License except as described by the License itself. No other terms or conditions may be applied to any Open Game Content distributed using this License.

3. Offer and Acceptance: By Using the Open Game Content You indicate Your acceptance of the terms of this License.

4. Grant and Consideration: In consideration for agreeing to use this License, the Contributors grant You a perpetual, worldwide, royalty-free, non-exclusive license with the exact terms of this License to Use, the Open Game Content.

\columnbreak

5. Representation of Authority to Contribute: If You are contributing original material as Open Game Content, You represent that Your Contributions are Your original creation and/or You have sufficient rights to grant the rights conveyed by this License.

6. Notice of License Copyright: You must update the COPYRIGHT NOTICE portion of this License to include the exact text of the COPYRIGHT NOTICE of any Open Game Content You are copying, modifying or distributing, and You must add the title, the copyright date, and the copyright holder's name to the COPYRIGHT NOTICE of any original Open Game Content you Distribute.

7. Use of Product Identity: You agree not to Use any Product Identity, including as an indication as to compatibility, except as expressly licensed in another, independent Agreement with the owner of each element of that Product Identity. You agree not to indicate compatibility or co-adaptability with any Trademark or Registered Trademark in conjunction with a work containing Open Game Content except as expressly licensed in another, independent Agreement with the owner of such Trademark or Registered Trademark. The use of any Product Identity in Open Game Content does not constitute a challenge to the ownership of that Product Identity. The owner of any Product Identity used in Open Game Content shall retain all rights, title and interest in and to that Product Identity.

8. Identification: If you distribute Open Game Content You must clearly indicate which portions of the work that you are distributing are Open Game Content.

9. Updating the License: Wizards or its designated Agents may publish updated versions of this License. You may use any authorized version of this License to copy, modify and distribute any Open Game Content originally distributed under any version of this License.

10. Copy of this License: You MUST include a copy of this License with every copy of the Open Game Content You Distribute.

11. Use of Contributor Credits: You may not market or advertise the Open Game Content using the name of any Contributor unless You have written permission from the Contributor to do so.

12. Inability to Comply: If it is impossible for You to comply with any of the terms of this License with respect to some or all of the Open Game Content due to statute, judicial order, or governmental regulation then You may not Use any Open Game Material so affected.

13. Termination: This License will terminate automatically if You fail to comply with all terms herein and fail to cure such breach within 30 days of becoming aware of the breach. All sublicenses shall survive the termination of this License.

14. Reformation: If any provision of this License is held to be unenforceable, such provision shall be reformed only to the extent necessary to make it enforceable.

15. COPYRIGHT NOTICE
Open Game License v 1.0 Copyright 2000, Wizards of the Coast, Inc.

</div>
