/*
		Version 3.0
		Stylesheet by Cryptonaut
		Last modified: 30 JAN 2015
		Details: This is a custom template made by /u/Cryptonaut. 
		Find out more on /r/Naut.

		--------------------------------------------------------------------------
		[Changelog]
		v1.0 - Initial Design - /r/Naut Template
		v1.5 - Update 1 - New colours, icons and a whole bunch of fixes.
		V1.6 - Update 2 - Adjustments to make Naut come back to the reddit UX.
		V1.7 - Update 3 - A whole lot of UI tweaks and fixes.
		V2.0 - Update 4 - Naut is now on GitHub, added nightmode and some fixes.
		V2.1 - Update 5 - Initial CSS3 update - Added transitions and minor responsive tweaks.
		V2.2 - Update 6 - Bugfixes and the return of the suggest-title button.
		V2.3 - Update 7 - Bugfixes, including the search button.
		V3.0 - Update 8 - Complete rewrite to include easier customizing of colours, 
						  sizes and margins, more transitions and animations and
						  much more.

		V3.0 - Update 9 - Complete UI revamp. See /r/Naut for more.

		-------------------------------------------------------------------------- */



	*, *:before, *:after { -webkit-box-sizing: border-box;-moz-box-sizing: border-box; box-sizing: border-box;}

	body {
		overflow-x: hidden;
		background-color: #eeeeee;
		min-width: 640px;
background: url(%%content%%)!important;
 background-repeat: repeat-x;
	}
		
		/* General Styles - Links / Buttons / Inputs */
		a {
			color: #4F8EF7;
			transition: color 0.15s ease;
		}

		input:not([type="submit"]), textarea {
			box-shadow: none!important;
			background-color: #fff!important;
			border: 1px solid #e5e5e5!important;
			color: #a01e5b!important;
			transition: all 0.15s ease!important;
		}

			input:hover, textarea:hover {
				border-color: #a01e5b!important;
			}

				input:focus, textarea:focus {
					outline: none!important;
					border-color: #a01e5b!important;
					color: #4D5763!important;
				}

		.btn, button {
			margin: 4px 8px 4px 0px;
			padding: 1px 12px 2px 12px;
			background-color: #fff;
			border: 1px solid #d4d4d4;
			border-radius: 2px;
			-moz-box-shadow: 0 1px 0 rgba(0, 0, 0, 0.05);
			-ms-box-shadow: 0 1px 0 rgba(0, 0, 0, 0.05);
			-webkit-box-shadow: 0 1px 0 rgba(0, 0, 0, 0.05);
			box-shadow: 0 1px 0 rgba(0, 0, 0, 0.05);
			color: #a01e5b;
			text-transform: capitalize;
			font-weight: bold;
			line-height: 26px;
			cursor: default;
			transition: all 0.15s ease;
			height: 29px;
		}

			.btn:hover, button:hover {
				-moz-box-shadow: 0 1px 0 0 rgba(0,0,0,0.27);
				-ms-box-shadow: 0 1px 0 0 rgba(0,0,0,0.27);
				-webkit-box-shadow: 0 1px 0 0 rgba(0, 0, 0, 0.27);
				box-shadow: 0 1px 0 0 rgba(0, 0, 0, 0.27);
				color: #a01e5b;
			}

				.btn:active, button:active {
					-moz-box-shadow: inset 0 2px 0 #d6d6d6;
					-ms-box-shadow: inset 0 2px 0 #d6d6d6;
					-webkit-box-shadow: inset 0 2px 0 #D6D6D6;
					box-shadow: inset 0 2px 0 #D6D6D6;
					background-color: #E5E5E5;
					color: #a01e5b;
				}

				.btn:focus, button:focus {outline: none;}



		/* Header */
		#header {
			margin: 0px;
			height: 0px;
			border: none;
		}


			#sr-header-area {
				background-color: #04091f;
 
				border: 0px solid;
				transition: all 0.15s ease;
				height: 24px;
				line-height: 23px;
			}

				#sr-header-area .width-clip {right: 300px;}
					body:not(.loggedin) #sr-header-area .width-clip {right: 340px;}

				#sr-header-area .sr-list {margin-right: 48px;}

				#sr-header-area .sr-bar a, #sr-more-link, #sr-header-area .separator, #sr-header-area .dropdown.srdrop .selected {
					background-color: transparent;
					color: rgba(255,255,255,0.6);
					transition: all 0.15s ease;
				}

					#sr-header-area:hover .sr-bar a, 
					#sr-header-area:hover #sr-more-link, 
					#sr-header-area:hover .seperator,
					#sr-header-area:hover .dropdown.srdrop .selected {color: rgba(255,255,255,1);}

					#sr-header-area .sr-bar a:hover, #sr-more-link:hover, #sr-header-area .dropdown.srdrop .selected:hover {
						background-color: transparent;
						border: 0px solid;
						transition: all 0.15s ease;
					}

						a.random.choice {
							padding-top: 2px;
							position: relative;
							display: inline-block;
							margin-top: -2px;
						}

				#sr-header-area .dropdown.srdrop .selected {
					margin: 0px 12px 0px 8px ;
					padding: 0px;
					background-image: none;
				}

					#sr-header-area .dropdown.srdrop .selected:hover {text-decoration: underline;}

					#sr-header-area .dropdown.srdrop .selected:after {
						position: relative;
						content: "▼";
						margin-left: 4px;
						font-size: 10px;
					}


					/* My Subreddits Dropdown */
					#sr-header-area .drop-choices.srdrop {
						background-color: #fff;
						border: none;
						box-shadow: 0px 2px 3px rgba(0, 0, 0, 0.15)
					}

						#sr-header-area .drop-choices a.choice {
							border-bottom: 1px solid #edeeee;
							color: #4D5763;
							padding: 2px;
						}

							#sr-header-area .drop-choices a.choice:hover {
								background-color: #f1f1f1;
							}




		#header-img.default-header, #header-img {
		 		display: none;
			}

				


                           #header .pagename {
		 		font-size: 0;
		 	}

		 		#header .pagename a {
		 			display: inline-block;
		 			color: #a01e5b;
		 			font-size: 2px;
		 			padding: 11px;
		 	
		 			position: relative;
		 			top: 3px;
		 			font-family: arial;
		 			margin: 0 4px;
		 			vertical-align: top;
		 			transition: background-color 0.25s ease;

					z-index: 99;
					width: 245px;
					height: 151px;
					background-image: url(%%header-img2%%);
					background-position: 0px 0px;
					position: absolute;
					top: 0px;
					margin: -50px 0px 0 0px;
		 		}

		 			#header .pagename a:hover {
		 				text-decoration: none;
		 				background-color: transparent;
		 			}

		 			#header .pagename a:before {
		 				display: none; 
		 				content: "/r/";
		 				font-size: 18px;
		 				font-variant: normal;
		 				letter-spacing: 1px;
		 			}


			/* Tabmenu (hot/new/top) */
			#header-bottom-left {
				position: absolute;
				top: 36px;
				left: 0px;
background-color: #a01e5b;
    position: absolute;
    width: 100%;
 height: 56px;
			}

				#header .tabmenu {
					 background-color: #a01e5b;
    border: medium none;
    left: 100px;
    margin: 0;
    padding-left: 150px;
   position: absolute;
 margin-top: 4px;
				}

					#header .tabmenu li a {
						display: inline-block;
						margin: 0px 4px;
						padding: 16px 16px;
						background-color: transparent;
transition: color 0.25s ease, background-color 0.25s ease;
						border: 0px;
						border-radius: 0px;

						color: rgba(255,255,255,0.6);
						text-transform: uppercase;
						font-weight: normal;
						font-size: 14px;
						font-family: Arial, sans-serif;
						
					}

						/* IF Headerimg is though */
						#header .tabmenu li a {
							color: #fff;
						}

						#header .tabmenu li a:hover {
							color: rgba(255,255,255,1);
							
						}

						#header .tabmenu li.selected a {
							padding: 16px 16px 14px 16px;
							background-color: transparent;
							border: 0px;
							border-bottom: 6px solid #fff;
							color: rgba(255,255,255,100);
							font-weight: bold;
						}

						

					.listing-page .tabmenu li:nth-of-type(3), .wiki-page .tabmenu li:nth-of-type(3),	/* Rising */
					.listing-page .tabmenu li:nth-of-type(4), .wiki-page .tabmenu li:nth-of-type(4),	/* Controversial */
					.listing-page .tabmenu li:nth-of-type(6), .wiki-page .tabmenu li:nth-of-type(6),	/* Self-serve advertising */
					.listing-page .tabmenu li:nth-of-type(9), .wiki-page .tabmenu li:nth-of-type(9)	/* gilded */
					{display:none;}


			


		
		/* Sidebar */
		.side {
				margin: 200px 16px 0px 0px;
			padding: 6px 16px;
			background-color: #fff;
			
background: none;

		}
		

			/* Objects from top to bottom */
			#header-bottom-right {
				position: absolute;
				top:0px;
				right: 0px;
				width: auto;
				max-width: 300px;
				height: 24px;
				background-color: transparent;
				font-size: 11px;
				color: rgba(255,255,255,0.45);
				padding: 5px 8px 4px 2px;

			}

				body:not(.loggedin) #header-bottom-right {max-width: 340px;}
				#header-bottom-right a {color: #fff;}
					#header-bottom-right a:hover {text-decoration: underline;}

				.user .userkarma {
					font-weight: normal;
					color: rgba(255,255,255,0.45);
					border: none;
					font-size: 9px;
					transition: all 0.15s ease;
				}

				.separator, .user {color: rgba(255,255,255,0.45);}


				#mail, #modmail {
					width: 16px;
					height: 14px;
					background-image: url(%%spritesheet%%) !important;
					background-repeat: no-repeat !important;
					background-color: transparent;
					transition: all 0.25s ease;
				}


					#mail {
						top: -2px;
						overflow: visible;
					}

						#mail.nohavemail {background-position: -32px -0px;}

						#mail.havemail {
							background-position: -32px -16px;
							opacity: 1;
						}

						.message-count {
							background-color: #f50;
							position: relative;
							top: -1px;
						}

						#mail.havemail:before {
							position: fixed;
							padding: 16px 24px;
							bottom: 24px;
							z-index: 100;
							background-color: #EA4848;
							border-radius: 2px;
							box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.24);
							color: #fff;
							width: 300px;
							height: 48px;
							left: 24px;
							content: "You have new messages!";
							text-indent: 0px;
							font-size: 14px;
							font-family: arial, sans-serif;
							line-height: 1;
							-webkit-transform:translateY(112px);
							transform:translateY(112px);
							transition: background-color 0.25s ease, box-shadow 0.25s ease;
							background-image: url(%%spritesheet%%);
							background-position: 269px -32px;
							background-repeat: no-repeat;
						}

							#mail.havemail:hover:before {
								background-color: #ec5b5b;
								box-shadow: 0px 3px 12px rgba(0, 0, 0, 0.48);
							}

								#mail.havemail:active:before {
									background-color: #c73d3d;
									box-shadow: 0px 4px 14px rgba(0, 0, 0, 0.76)
								}


					#modmail {top: -3px;}

						#modmail.nohavemail {background-position: -48px -0px;}
						#modmail.havemail {background-position: -48px -16px;opacity: 1;}




				/* preferences & logout icons */
				#header-bottom-right a.pref-lang, .loggedin .logout a{
					background-position: -0px -16px;
					background-image: url(%%spritesheet%%);
					width: 16px;
					height: 14px;
					display: inline-block;
					text-indent: -9999px;
					margin: 0px;
					position: relative;
					top: -1px;
					transition: all 0.25s ease;
				}

					.loggedin .logout a {background-position: -16px -0px;}

				.side:after {
					display: block;
					margin: 10px 0px;
					padding: 10px 0px;
					color: #5B92FA;
					content: "";
					text-transform: none;
					font-size: 16px;
					font-family: arial,sans-serif;
					position: absolute;
					width: 300px;
					text-align: center;
					right: 16px;
				}

			/* Search */
			#search {
				position: absolute;
				right: 16px;
				top: 96px;
				z-index: 1;
				width: 300px;
background-color: none !important;
background: url(%%Searchbox%%);
			}

				#search input[type=text] {
					padding: 10px 25px 10px 16px;
					border: 0px solid !important;
					
					
					transition: all 0.25s ease;

}
				

					

						#search input[type=text]:focus {
							border-radius: 2px 2px 0px 0px;
						}

						#search input[type=text]:focus:hover {box-shadow: 0px 1px 5px rgba(0,0,0,0.24) !important;}

						#search input[type="text"]:-moz-placeholder {font-size: 0;}
						#search input[type="text"]::-webkit-input-placeholder {font-size: 0;}
						#search input[type="text"]:-ms-input-placeholder {font-size: 0;}

						#search input[type="text"]:-moz-placeholder::after {
						    font-size: 14px;
						    content: "Search..";
						    position: relative;
						    top: 1px;
						}

						#search input[type="text"]::-webkit-input-placeholder::after {
						    font-size: 14px;
						    content: "Search..";
						    position: relative;
						    top: 1px;
						}

						#search input[type="text"]:-ms-input-placeholder::after {
						    font-size: 14px;
						    content: "Search..";
						    position: relative;
						    top: 1px;
						}


						#search input[type=text]::-webkit-input-placeholder {color:#B3B3B3;}
						#search input[type=text]:-moz-placeholder {color:#B3B3B3;}
						#search input[type=text]::-moz-placeholder {color:#B3B3B3;} 
						#search input[type=text]:-ms-input-placeholder {color:#B3B3B3;}

						#search input[type=submit] {
							height: 32px;
							width: 32px;
							margin-left: -38px;
							background-image: url(%%spritesheet%%);
							background-position: -193px -231px;
							background-repeat: no-repeat;
							border:none !important;
							border-radius: 16px;
							background-color: rgba(0,0,0,0.00);
							transition: background-color 0.15s ease;
						}

							#search input[type=submit]:hover {
								background-image: url(%%spritesheet%%);
								background-position: -193px -231px;
								background-repeat: no-repeat;
								background-color: rgba(0,0,0,0.05);
							}

				/* Expando */
				#search #searchexpando {
					background-color: #f2f2f2;
					border: none;
					border-radius: 0px 0px 2px 2px;
					margin-top: -5px;
					padding-top: 10px;
					padding-left: 0px;
					padding-right: 0px;
					height: 57px;
					line-height: 45px;
				}

					#search #searchexpando label {
						padding: 18px 8px 17px 8px;
						cursor: pointer;
						transition: all 0.1s ease;
					}

						#search #searchexpando label:hover {background-color: rgba(0,0,0,0.1);}
							#search #searchexpando label:active {background-color: rgba(0,0,0,0.25);}

					#search #searchexpando p {display: none !important;}


			/* Submit Button */
			.morelink {
				position: absolute;
				top: 148px;
				
				
				background-image: url(%%spritesheet%%) !important;
				background-position: 268px -214px!important;
				background-repeat: no-repeat !important;
background: url(%%Searchbox%%)!important;
    background-size: 100% !important;
				right: 16px;
				width: 300px;
				height: 73px;
				
				line-height: 36px;
				border: none;
				text-align: left;
				padding: 0px 16px;
				transition: all 0.25s ease;
				font-family: verdana, arial, sans-serif;
			}	

				

					.morelink:active {
						background-color: #c3c3c3;
						box-shadow: 0px 8px 12px rgba(0,0,0,0.60);
					}


				.morelink a {
					color: #a01e5b !important;
					font-weight: bold;
					font-size: 14px;
					letter-spacing: 0px;
width: 100%;
margin-top: 18px;
 text-align: center;
				}


				.morelink:after {
					content: "Please remember to read the rules. Thank you!";
					padding: 16px;
					width: 300px;
					position: absolute;
					right: 0px;
					margin-top: 0px;
					display: block;
					background-color: #a01e5b !important;
					color: #ffffff;
					letter-spacing: 0px;
					z-index: 100;
					opacity: 0;
					transition: all 0.25s ease;
					transition-delay: 0s;
					font-weight: normal;
					line-height: 1.4em;
					border-radius: 2px 2px 0px 0px;
			
					visibility: hidden;
					pointer-events: none;
				}

					.morelink:hover:after {
						
						opacity: 100;
						visibility: visible;
						transition-delay: 0.25s;
background-color: a01e5b;
color: a01e5b !important;
					}

				/* Restricted button */
				.disabled .morelink {
					box-shadow: none !important;
					background-color: #CFCFCF;

				}

					.disabled .morelink a {color: #4d5763;}

					.disabled .morelink:after {
						content: "You must be approved by the moderators in order to submit.";
						background-color: #CFCFCF;
						color: #4d5763;
					}


			.account-activity-box, .sidebox.create, .morelink .nub,.sidebox.submit.submit-text {display: none;}


			/* Login form */
			.login-form-side {border: none;}

				.login-form-side input[type=text], .login-form-side input[type=password] {width: 128px;}


				
			/* Redditname + Subscibers & Here right now */
			

.titlebox h1 a {
    color: #a01e5b;
}
			.titlebox span.subscribers, .titlebox .users-online, .titlebox .number {
				color: #999999;
				font-size: 12px;
				position: relative;
				top: -2px;
				left: -2px;
			}

				div.titlebox span.word {display: none;}
				.titlebox .users-online {display: inline;}
				.titlebox .users-online:before {display: none;}
				div.titlebox span.number:after {content: " People of Tomorrow,";}
				.titlebox .users-online .number {font-style: italic;}
				.titlebox .users-online .number:before {content: "";}
				.titlebox .users-online .number:after {content: " present";}
				.titlelebox .word {display: none;}
				.titlebox .users-online, .titlebox .number {cursor: text;}	


			.titlebox .tagline {
					font-size: 12px;
					margin: 0;
				}

					.titlebox .tagline:after {

						
   padding-top: 16px;		}

				.titlebox .tagline a.flairselectbtn {
					color: #4F8EF7;
				}	
				.titlebox .tagline a.flairselectbtn:after {content: " flair"}
				.titlebox .tagline .flair:before {content: "";}


			.titlebox form.toggle, .leavemoderator, .titlebox .tagline a.author, .sidebox .subtitle {display: none;}

			/* Subscribe Button */
			.titlebox .fancy-toggle-button {position: relative;}

			.titlebox .fancy-toggle-button .add, .fancy-toggle-button .remove {
				text-indent: -9999px;
				height: 48px;
				width: 48px;
				position: absolute;
				right: -268px;
				top: -55px;
				background-image: none;
				border-radius: 32px;
				background-color: #51A3E8;
				border: 0px solid;
				
				background-image: url(%%spritesheet%%);
				transition: all 0.25s ease, background-position 0.25s ease, background-color 0.5s ease;
				outline: none !important;
			}

		

					.titlebox .fancy-toggle-button .add:active, .fancy-toggle-button .remove:active {
						
					}

				.titlebox .fancy-toggle-button .add {
					background-color: #516AE8;
					background-position: -208px -147px;
				}

					.titlebox .fancy-toggle-button .add:hover {background-color: #5A72EE;}

						.titlebox .fancy-toggle-button .add:active {
							background-color: #fff;
							background-position: -208px -192px
						}

				.fancy-toggle-button .remove {
					background-color: transparent;
					background-position: -208px -192px;
				}

					

						.fancy-toggle-button .remove:active {
							background-color: #5A72EE;
							background-position: -208px -144px
						}


				/* Hover Message */
				.titlebox .fancy-toggle-button .add:after, .fancy-toggle-button .remove:after {
					display: block;
					visibility: hidden;
					position: absolute;
					z-index: 1000;
					right: -26px;
					margin-top: 16px;
					padding: 12px;
					background-color: rgba(79, 77, 192, 0);
					border: none;
					border-radius: 2px;
					color: rgba(255, 255, 255, 0);
					text-align: center;
					letter-spacing: 1px;
					font-weight: normal;
					font-size: 13px;
					transition: all 0.25s ease;
					pointer-events: none;
					text-indent: 0;
					box-shadow: 0px 0px 0px rgba(0,0,0,0.00);
				}

					.titlebox .fancy-toggle-button .add:after {content: "Subscribe!";}
					.titlebox .fancy-toggle-button .add:hover:after {
						visibility: visible;
						margin-top: 40px;
						color: #ffffff;
						background-color: #a01e5b !important;
						box-shadow: 0px 1px 5px rgba(0,0,0,0.24);
					}


					.titlebox .fancy-toggle-button .remove:after {content: "Unsubscribe";}
					.titlebox .fancy-toggle-button .remove:hover:after {
						visibility: visible;
						background-color: #a01e5b !important;
						color: #fff;
						margin-top: 40px;
						box-shadow: 0px 1px 5px rgba(0,0,0,0.24);
					}





			/* Text */
			.side .md .-blocks, .side .md .-lists, .side .md pre, .side .md blockquote, .side .md table, .side .md p, .side .md ul, .side .md ol {
				color: #4D5763;
 margin-top: 10px;
				font-size: 13px;
				font-family: Arial, sans-serif;
				line-height: 1.3333333333333333em;
			}

				.side .titlebox .md h1 {
					line-height: 18px;
					margin: 0.5em 0 0 0 !important;
				}

				.side .titlebox .md h2 {
					margin: 16px 0px 2px 0px;
				}

				/* Buttonstyle one */


				.side .titlebox .md h3 a {
					padding: 25px 16px;
text-align: center;
					width: 100%;
					border-radius: 2px;
background: url(%%Searchbox%%)!important;
    background-size: 100% !important;
				right: 16px;
				width: 300px;
				height: 73px;
					background-color: #background-color: #a01e5b;
					font-family: verdana,arial,sans-serif;
					
					color: #a01e5b;
					letter-spacing: 0;
					display: block;
					margin: 1.5em -15px;
					font-size: 14px;
				}

					

						.side .titlebox .md h3 a:active {
							background-color: #4059DB;
							box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.54);
						}

				.side .titlebox .md h4 a, .wiki-page .wiki-page-content .md.wiki h4 {
					padding: 12px 16px;
					background-color: #FFF;
					border: 1px solid #D4D4D4;
					border-radius: 2px;
					box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.12);
					color: #737373;
					font-weight: bold;
					transition: all 0.15s ease;
					display: block;
					margin: 1.5em 0em;
					font-size: 12px;
				}

					.side .titlebox h4 a:hover, .wiki-page .wiki-page-content .md.wiki h4:hover {
						box-shadow: 0px 3px 8px rgba(0, 0, 0, 0.24);
						color: #4D5763;
					}

						.side .titlebox h4 a:active, .wiki-page .wiki-page-content .md.wiki h4:active {
							box-shadow: inset 0 2px 0 #D6D6D6;
							background-color: #E5E5E5;
							color: #999;
							box-shadow: 0px 6px 12px rgba(0, 0, 0, 0.36);
						}


				.md hr {border: solid 1px #e5e5e5;}


			.titlebox .bottom {display: none;}


			/* Mod Box */
			.side #moderation_tools {

			}

				.side #moderation_tools .title {

				}

					.side #moderation_tools .title h1 {
						text-transform: capitalize;
						color: #4D5763;
					}

					.side #moderation_tools .title .collapse-button {
						color: #4D5763;
						vertical-align: middle;
						border-radius: 1px;
						border: 1px solid #d8d8d8;
					}

				.side .sidecontentbox .content {
					border: none;
					padding: 8px 0px;
				}


			/* Ads */
			#ad_sponsorship, #ad-frame, #ad_main {margin-left: -16px;}
			#ad_sponsorship {margin-top: -18px;border-radius: 2px 2px 0px 0px;}

			/* Recently viewed links */
			.gadget .midcol {width: 38px;}





		/* Body Content - Frontpage */
		.content {
			margin: 96px 16px 0px 16px;
			padding: 0px;
		}	

			.content:before {
				height: 166px;
				top: 0px;
				position: absolute;
				width: 100%;
				left: 0px;
				right: 0px;
				background-color: #3A3D4D;
				background-image: url(%%headerimg%%);
				background-repeat: no-repeat;
				background-position: 50% 0%;
				content: "";
				text-indent: -9999px;
				z-index: -1;
			}

				@media only screen and (min-width : 1921px) {
					.content:before {background-size: cover;}
				}

			.sitetable {
				margin-right: 316px;
				box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.16);
				position: relative;
			}

				.link {
					margin: 0px;
					background-color: #ffffff;


				}

					/* Objects on the link from left to right */
					body >.content .link .rank, .rank-spacer {display: none;}

					/* Voting Arrows */
					.link .midcol {
						width: 36px !important;
						margin: 15px 14px 0px 11px;
						overflow: visible;
						height: 60px;
					}
						.link .score {
							line-height: 16px;
							font-size: 12px;
							margin: 1px 0px 1px 0px;
						}

							.link .score.likes {color: #a01e5b;}
							.link .score.dislikes {color: #c3c3c3;}

						.arrow {
							margin: 0px 0px 0px 2px;
							background-image: url(%%spritesheet%%) !important;
							background-color: transparent;
							width: 33px;
							border-radius: 2px;
							transition: background-color 0.25s ease;
						}

							.arrow:hover {background-color: rgba(0,0,0,0.05);}

							/* Upvotes */
							.arrow.up {
								height: 20px;
								background-position: -64px 0px;
								transition: background-color 0.25s ease;
							}

								.arrow.upmod {
									height: 20px;
									background-position: -128px 0px;
									position: relative;
								}

									.arrow.upmod:focus:after {
									    font-size: 13px;
									    font-weight:bold;
									    font-family: arial, sans-serif;
									    position: absolute;
									    left:8px;
									    opacity: 1;
									    z-index:100;
									    white-space: nowrap;
									    content: "+1";
									    bottom: 15px;
									    color:#a01e5b;
									    -webkit-animation: upvote 0.8s ease-out forwards;
									}

							/* downvotes */
							.arrow.down {
								height: 20px;
								background-position: -160px 0px;
								transition: background-color 0.25s ease;
							}
								.arrow.downmod {
									height: 20px;
									background-position: -224px 0px;
								}


								/* Hover Message on Downvote */
								.arrow.down:after {
									display: block;
									visibility: hidden;
									position: absolute;
									z-index: 1000;
									margin-top: -6px;
									margin-left: 32px;
									padding: 12px;
									background-color: #a01e5b;
									border: none;
									border-radius: 2px;
									color: #ffffff;
									content: "For content that does not contribute to any discussion.";
									text-align: center;
									letter-spacing: 1px;
									font-weight: normal;
									font-size: 13px;
									transition: all 0.25s ease;
									pointer-events: none;
								}

									.arrow.down:hover:after {
										visibility: visible;
										background-color: #a01e5b;
										color: #FFF;
										margin-left: 48px;
									}

					/* Thumbnails */
					.thumbnail {
						max-width: 64px;
						max-height: 56px;
						margin: 16px 16px 0px 0px;
						background-color: #ddd;
					}

						.thumbnail a img, .thumbnail.self, .thumbnail.default {height: 56px;}

						.thumbnail.self 	{	background: url(%%spritesheet%%) -073px -80px;}
						.thumbnail.default 	{	background: url(%%spritesheet%%) -143px -80px;}
						.thumbnail.nsfw 	{	background: url(%%spritesheet%%) -003px -140px;}

					/* Linkflairs */
					.linkflairlabel {
						padding: 1px 6px 1px 6px;
						height: 17px;
						border-radius: 2px;
						border: 0px solid;
						color: #fff;
						font-weight: bold;
						font-style: normal;
						font-variant: normal;
						font-size: 13px;
						font-family: Arial, sans-serif;
						cursor: default;
						vertical-align: middle;
						position: relative;
						top: -2px;
						background-color: #4F8EF7;
					}

						.linkflair-inspiration .linkflairlabel {
							background-color: #ea4848;
							color: #fff;
						}

							.linkflair-inspiration .thumbnail.self {background: url(%%spritesheet%%) -143px -140px;}

						.linkflair-waywo .linkflairlabel {
							background-color: #516ae8;
							color: #fff;
						}

							.linkflair-waywo .thumbnail.self {background: url(%%spritesheet%%) -73px -140px;}


						.linkflair-mod .linkflairlabel {
							background-color: #65B354;
							color: #fff;
						}

							.linkflair-mod a {color: #65B354!important;}
							.linkflair-mod .thumbnail.default, .linkflair-mod .thumbnail.self {background: url(%%spritesheet%%) -3px -80px !important;}

					/* Submission Title */
					.link .title {
						margin: -2px 0px 0px 0px;
						font-size: 18px;
						font-family: Arial, sans-serif;
						overflow: visible;
						transition: all 0.15s ease;
					}

						body .content .sitetable .link .title a:hover {color: #4F8EF7;}

						.link .entry {
							padding: 15px 32px 14px 0px;
							border-bottom: 2px solid #b69959;
							margin-left: 0;
						}

						/*Unvisited*/	.thing .title.loggedin.click, .thing .title.click, .thing .title.loggedin, .thing .title {color:#4F8EF7;}
						/*Visited  */	.content .thing .title:visited, .content .thing.visited .title {color: #b3b3b3;}
						/*Clicking */	.thing .title.loggedin.click:visited, .thing .title.click:visited {color:#7D5D8A;}




					/* Domain */
					.link .domain {visibility: hidden;}

						.link .domain a {
							visibility: visible;
							position: relative;
							top: -1px;
							color: #b3b3b3;
							transition: all 0.15s ease;
						}

							.link .domain a:hover {
								color: #4F8EF7;
								text-decoration: none;
							}

					.approval-checkmark {cursor: default;}

					/* Expando Button */
					.expando-button, .expando-button.image, .expando-button.video-muted {
						position: relative;
						margin: 2px 6px 2px 0px !important;
						width: 16px;
						height: 16px;
						border-radius: 2px
						background-color: #fff;
						background-image: url(%%spritesheet%%) !important;
						border: 1px solid #e9e9e9;
						cursor: pointer;
					}



						.expando-button:hover {
							background-color: #4F8EF7;
							border-color: #4F8EF7;
						}

						.expando-button.selftext.collapsed 					{background-position: -032px -32px;}
						.expando-button.selftext.collapsed:hover 			{background-position: -048px -32px;}
			
						.expando-button.selftext.expanded 					{background-position: -064px -32px;}
						.expando-button.selftext.expanded:hover 			{background-position: -080px -32px;}
			
						.expando-button.video.collapsed 					{background-position: -096px -32px;}
						.expando-button.video.collapsed:hover				{background-position: -112px -32px;}
			
						.expando-button.video.expanded 						{background-position: -064px -32px;}
						.expando-button.video.expanded:hover 				{background-position: -080px -32px;}

						.expando-button.image.collapsedExpando				{background-position: -160px -32px;}
						.expando-button.image.collapsedExpando:hover 		{background-position: -176px -32px;}

						.expando-button.image.expanded						{background-position: -064px -32px;}
						.expando-button.image.expanded:hover				{background-position: -080px -32px;}

						.expando-button.image.gallery.collapsedExpando		{background-position: -128px -32px;}
						.expando-button.image.gallery.collapsedExpando:hover{background-position: -144px -32px;}

						.expando-button.image.gallery.expanded				{background-position: -064px -32px;}
						.expando-button.image.gallery.expanded:hover		{background-position: -080px -32px;}

						.expando-button.video-muted.collapsed				{background-position: -208px -32px;}
						.expando-button.video-muted.collapsed:hover			{background-position: -224px -32px;}

						.expando-button.video-muted.expanded				{background-position: -064px -32px;}
						.expando-button.video-muted.expanded:hover			{background-position: -080px -32px;} 


					/* Expando Text */
					.link .usertext .md {
						margin-top: 10px;
						padding-top: 3px;
						padding-left: 0;
						background-color: transparent;
						border: 0px solid;
						border-top: 1px solid #F7F7F7;
						border-radius: 0px;
						color: #4D5763;
					}


					/* Submitted X ago by.. */
					.link .entry .tagline {
						margin-top: 4px;
						color: #b3b3b3;
						font-size: 12px;
						font-family: arial, sans-serif;
						transition: all 0.15s ease;
					}

						.link .entry .tagline a {color: #4d5763;}

						.link .entry .tagline:first-letter {text-transform: capitalize;}
						.link .entry .tagline time {cursor: help;}
						.link .entry .tagline a:hover {color: #4F8EF7;text-decoration: none;}
						.link .entry .tagline a.author {margin-right: inherit;}

						.link .entry .tagline .userattrs {visibility: hidden;}
						.link .entry .tagline .userattrs a {
							visibility: visible;
							font-size: 10px;
							padding: 1px 3px 1px 2px;
							margin-left: 2px;
							background-color: #f00;
							color: #fff !important;
							vertical-align: middle;
							border-radius: 1px;
							position: relative;
							top: -1px;
							cursor: help;
						}

							.link .entry .tagline .userattrs a.moderator {background-color: #65B354;}
							


						.RESUserTagImage {
							height: 10px !important;
							background-image: url(%%spritesheet%%) !important;
							background-position: -192px -34px !important;
							opacity: 0.25 !important;
							margin-left: 2px !important;
							transition: opacity 0.15s ease;
							margin-top: 1px !important;
						}

							.RESUserTagImage:hover {opacity: 1 !important;}


					/* Comment / Share / Report */
					.link .flat-list {margin-top: 3px;}

						.link .entry .buttons li a {
							padding: 0 1px;
							color: #b3b3b3;
							font-weight: normal;
							font-size: 13px;
							font-family: Arial, sans-serif;
							transition: all 0.15s ease;
						}
		
							.link .entry .buttons li a:hover {color: #4F8EF7;text-decoration: none;}
		
							.nsfw-stamp acronym {
								padding: 2px 3px;
								background-color: transparent;
								border-color: #e82e63 !important;
								border-radius: 2px;
								color:#e82e63;
								opacity: 100;
								cursor: help;
							}
		
							.link .entry .buttons li a.comments {
								color: #4F8EF7;
								font-weight: bold !important;
								opacity: 100 !important;
								transition: all 0.25s ease-in-out !important;
							}

								.link .entry li .comments:hover {
									text-decoration: none;
								}


							/* Save Category popup */


							/* Reporting Comment */
							.link .entry .report-form {
								position: fixed;
								top: 35%;
								left: 50%;
								margin-left: -150px;
								margin: 0;
								padding: 24px;
								background-color: #fff;
								z-index: 100;
								box-shadow: 0px 0px 16px rgba(0, 0, 0, 0.24);
								border: none;
								border-radius: 2px;
							}

								.link .entry .report-form .reason-prompt {
									font-size: 16px;
									color: #4D5763;
									padding-bottom: 8px;
									display: block;
								}

									.link .entry .report-form .reason-prompt:first-letter {text-transform: capitalize;}

									.link .entry .report-form .reason-prompt li {
										padding: 4px 4px 4px 0px;
										display: block;
									}
										.link .entry .report-form li label {
											padding: 4px 4px 4px 0px;
											cursor: pointer;
											display: block;
											color: #4D5763;
											text-transform: capitalize;
										}

											.link .entry .report-form li label:hover {background-color: rgba(0,0,0,0.05);}
											.report-form input[name="other_reason"] {padding: 8px;}


								/*	.link .entry li .comments:hover .newComments {color: #fff !important;} */

								/* Flair */
								.link .entry .buttons li a.flairselectbtn {color: #4F8EF7;}

								/* RES L+C */
								.link .entry .buttons li .redditSingleClick {
									padding: 0 1px;
									color: #b3b3b3;
									font-weight: normal;
									font-size: 13px;
									font-family: Calibri, Candara, Segoe, "Segoe UI", Optima, Arial, sans-serif;
									transition: all 0.15s ease;
								}


					/* Reported & Spam/Remove/Approves */
					.entry .buttons li.reported-stamp {
						background-color: transparent;
						border: 1px solid #EDEEEE!important;
						border-radius: 20px;
						color: #4A4F57;
						line-height: 16px;
					}


					a.pretty-button.negative, a.pretty-button.neutral, a.pretty-button.positive {
						background-image: none;
						border: 1px solid;
						border-radius: 20px;
						box-shadow: inset 0px 0px 0px rgba(0, 0, 0, 0.25);
						color: #fff;
						line-height: 15px;
						transition: all 0.25s ease;
					}

						a.pretty-button.negative {background-color: #fb797e;border-color: #fb797e;}
							a.pretty-button.negative:hover {background-color: #fc535a;border-color: #fc535a;}

						a.pretty-button.neutral {background-color: #dddddd;border-color: #dddddd;color: #4A4F57;}
							a.pretty-button.neutral:hover {background-color: #ececec;border-color: #ececec;}

						a.pretty-button.positive {background-color: #1ecd97;border-color: #1ecd97;}
							a.pretty-button.positive:hover {background-color: #22e1a6;border-color: #22e1a6;}


						a.pretty-button.positive.pressed, a.pretty-button.neutral.pressed, a.pretty-button.negative.pressed {background-image: none;box-shadow: inset 0px 3px 1px rgba(0, 0, 0, 0.15);}

					/* Last Clicked */
					.link.last-clicked {
						background-color: #F2F2F2;
						border: none;
					}


					/* Sticky Post */
					.thing.stickied {
						border-radius: 2px 2px 0px 0px;
					}

						.thing.stickied a.title, .thing.stickied a, .thing.stickied .entry li .comments {color: #65b354!important;}					
						.thing.stickied .expando-button:hover {background-color: #65b354!important;border-color: #65b354!important;}
						.tagline .stickied-tagline {color: #b3b3b3;cursor: help;}
						.thing.stickied .domain {display: none;}

					/* Ad */
					.link.promotedlink.promoted {
						margin-right: 0;
						background-color: #EFF7FF;
						border: none;
					}

						.organic-listing {  
							background-color: white!important;  
							padding: 0;  
							z-index: 9999;  
							position: relative;  
							margin-bottom: 0px;  
							margin-right: 316px;  
							border: none;  
							border-radius: 2px 2px 0px 0px; 
						} 


					/* Compressed post */
					.link.compressed {margin: 0;}

						.link.compressed .entry {padding: 11px 32px 9px 0px;}
						.link.compressed .title {margin: 0;}
						body>.content .link.compressed .midcol {
							height: auto;
							margin: 8px 0px 0px 4px;
						}

					/* Flair Selector */
					.flairselector {
						position: fixed;
						top: 20% !important;
						left: 50% !important;
						margin-left: -125px;
						padding: 32px !important;
						width: 250px !important;
						border: none;
						border-radius: 2px;
						box-shadow: 0px 0px 16px rgba(0, 0, 0, 0.64);
						max-height: 400px;
					}

						.flairselector.drop-choices.active {border: 1px solid #e2e2e2;}

						.flairselector h2 {
							margin-bottom: 4px;
							background-color: transparent;
							color: #4F8EF7;
							text-align: left;
							text-transform: capitalize;
							font-weight: normal;
							font-size: 18px;
						}

						.flairoptionpane {
							max-height: 600px;
							text-align: left;
						}

							.flairselector .flairoptionpane ul li {
								padding: 0px !important;
							}

								.flairoptionpane ul li .linkflair {
									text-align: left;
									padding: 0px;
								}

									.flairoptionpane ul li .linkflair:hover, .flairselector li:hover {background-color: #F5F8F9;border: 0px solid;}

									.flairoptionpane ul li .linkflair span.linkflairlabel {
										margin: 8px 0px;
										line-height: 1.35;
										margin-right: 6px;
									}

									.flairoptionpane ul li .linkflair a.title {
										font-size: 18px !important;
										opacity: 100 !important;
										color: #4F8EF7 !important;
									}

						.flairselector form {
							padding-top: 12px;
							border-top: 1px solid #F7F7F7;
						}

							.flairselector form .flairselection {text-align: left;}

								.flairselector form .flairselection:before {
									display: block;
									content: "Selected Flair:";
									color: #b3b3b3;
								}

								.flairselector form .flairselection .linkflair a.title {
									font-size: 18px !important;
									opacity: 100 !important;
									color: #4F8EF7 !important;
									cursor: default;
								}
		
								.flairselector form .flairselection .flairremove {
									padding: 4px 0px;
									margin-bottom: 8px;
									visibility: hidden;
									display: block !important;
								}
		
									.flairselector form .flairselection .flairremove a {
										visibility: visible;
										opacity: 100 !important;
										color: #4F8EF7 !important;
										margin-left: -4px;
										text-transform: capitalize;
									}

										.flairselector form .flairselection .flairremove a:first-letter {text-transform: capitalize;}
		
										.flairselector form .flairselection .flairremove a:hover {text-decoration: underline !important;}

						.flairselector .error {text-align: left;}
							.flairselector .error:first-letter {text-transform: capitalize;}
							.flairselector .error:after {
								display: block; 
								color: #b3b3b3;
								content: "Go to /r/.../about/flairs.";
							}

						.flairselector img {
							position: relative;
							left: 50%;
							margin-left: -9px;
							opacity: 0.5;
						}

							.flairselector .flairoptionpane ul li {
								margin: 4px 0px;
							}

								.flairselector li.selected {border: none;background-color: }
								.flairselector .flairoptionpane ul li.flairsample-right {
									padding: 5px 0px !important;
									border: none;
								}

								.flairselector li a, .flairselector form .flairselection a.author {
									color: #b3b3b3 !important;
									font-size: 11px;
								}


						.flairselector:before {
							display: block;
							position: fixed;
							top: 0px;
							left: 0px;
							z-index: -2;
							overflow: hidden;
							width: 100%;
							height: 100%;
							background-color: rgba(255, 255, 255, 0.75);
							content: "";
							cursor: default;
							transition: all 0.25s ease;
							pointer-events: none;
						}



					/* Unvotable Message */
					.unvotable-message {
						border: 0px solid;
						color: #b3b3b3;
					}

						.unvotable-message:first-letter {text-transform: capitalize;}

					/* RES Selection */
					.res .RES-keyNav-activeElement {
						outline: 0px dashed #E0E0E0 !important;
						transition: all 0.35s ease;
					}

						.res .entry {transition: all 0.15s ease;}

						div.RES-keyNav-activeElement, 
						div.commentarea div.RES-keyNav-activeElement.entry div.noncollapsed {
							background-color: transparent !important;
							padding-left: 8px !important;
							border-left: 2px solid #4F8EF7;
						}

							div.commentarea div.RES-keyNav-activeElement .md {
								background-color: transparent !important;
							}

								.res .commentarea .thing {
									padding: 16px 16px 0px 14px !important;
								}

									.res .commentarea .entry .flat-list {
										padding-bottom: 16px;
									}


					/* RES Tag dialog + RES Tag */
					.userTagLink.hasTag, #userTaggerPreview {
						font-size: 11px !important;
						border-radius: 0px !important;
						border: 0px solid !important;
						margin-top: 0px !important;
						margin-left: 4px !important;
					}

					.RESDialogSmall {
						border: none;
						box-shadow: 0px 2px 3px #DDD;
					}

						.RESDialogSmall > h3 {
							color: #4F8EF7;
							background-color: #FFF;
							border-bottom: 1px solid #EDEDED;
							height: 36px;
							padding-top: 9px;
						}

						.RESCloseButton {
							line-height: 19px;
							height: 22px;
							width: 22px;
							transition: all 0.15s ease;
						}

							.RESCloseButton:hover {
								border: 1px solid #D7D9DC;
							}

						#userTaggerToolTip input[type=text], #userTaggerToolTip select {
							line-height: 22px;
							padding-left: 4px;
							border: 1px solid #E5E5E5!important
						}

						.toggleButton {
							line-height: 0.8;

						}

							.toggleButton .toggleOn {
								border-radius: 0px;
								border: 1px solid #4F8EF7;
								background-color: #4F8EF7;
								color: #fff;
								text-transform: capitalize;
							}

							.toggleButton .toggleOff {
								border-radius: 0px;
								border: 1px solid #D7D9DC;
								background-color: transparent;
								text-transform: capitalize;
							}

							#userTaggerToolTip input[type=submit] {bottom: 10px !important;}

				/* Sorting Menu (Top links today/this week/ever) */
				.top-page .content .menuarea .drop-choices.lightdrop {
				display:inline;
				visibility:visible;
				}

				.top-page .menuarea .spacer {overflow: visible;}

				.top-page .content .menuarea .drop-choices.lightdrop a.choice, .top-page .content .menuarea .drop-choices.lightdrop form {display:inline;}
				.top-page .content .menuarea .dropdown-title.lightdrop {visibility: hidden;}

				.top-page .content .menuarea {
					border-bottom: 0px;
					padding: 0;
					margin: 0;
					height: 36px;
				}

					.top-page .content .menuarea .dropdown.lightdrop .selected {
						z-index: 1002;
						position: relative;
						left: -68px;
						top: 11px;
						background: none;
						text-decoration: none;
						text-transform: capitalize;
						font-size: 12px;
						pointer-events: none;
						padding: 10px 16px 10px 16px;
						background-color: #5A72EE;
						overflow: visible;
						color: #FFF;
					}

					.top-page .content .menuarea .drop-choices.lightdrop {
						padding: 10px 16px 10px 104px;
						margin-left: 16px;
						margin-top: 1px;
						border-radius: 2px 2px 0px 0px;
						border: none;
						border-bottom: 1px solid #E0E1E2;
						width: calc(100% - 348px);
						box-shadow: none;
					}

						.top-page .content .menuarea .drop-choices.lightdrop a.choice {
							padding: 10px;
							color: #4D5763;
							transition: all 0.25s ease;
						}

							.top-page .content .menuarea .drop-choices.lightdrop a.choice:[href*="/?t=all"] {border-right: 0px solid;}
							.top-page .content .menuarea .drop-choices.lightdrop a.choice:hover {background-color: #F5F8F9;}

							.top-page .content .menuarea .drop-choices.lightdrop a.choice.selected {
								background-color: #4f8ef7;
								color: #fff;
							}

					/* RES Popup */
					.guider {
						border: none;
						box-shadow: 0px 2px 3px #DDD;
					}

						.guider_content {}

							.guider_content h1 {color: #4F8EF7;}

							.guider_button {
								font-size: 11px;
								border: none;
								background-image: none;
								background-color: #4F8EF7;
								transition: all 0.15s ease;
							}

								.guider_button:hover {background-color: rgba(79, 142, 247, 0.75);}

							.guider_close {}

								.x_button {
									transition: all 0.25s ease;
									box-shadow: 0px 1px 4px rgba(0, 0, 0, 0.00);
								}

									.x_button:hover {box-shadow: 0px 1px 4px rgba(0, 0, 0, 0.15);}

				/* Infobar (Default yellow announcement bar) */
				.content .infobar {
					margin: 0px 0px 16px 0px;
					padding: 8px 16px;
					line-height: 26px;
					border: none;
					margin-right: 316px;
					background-color: #516AE8;
					color: #fff;
					box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.24);
					border-radius: 2px;
				}

					.infobar .md {color: #fff;}

					.content .infobar:first-letter {text-transform: capitalize;}

					/* Welcome infobar */
					.content .infobar.welcome {line-height: inherit;height: 86px;}
						.content .infobar.welcome h1 {color: #4d5763;}

					.commentarea .infobar {
						padding: 8px 16px;
						line-height: 16px;
						margin-right: 0;
					}

						.commentarea .infobar a {color: rgba(0,0,0,0.54);font-weight: bold;}

				/* Noresults image */
				#noresults {
					margin: 0;
					position: absolute;
					top: 72px;
					width: 100%;
					height: 312px;
					background: transparent url(%%noresults%%) no-repeat 50% 50%;
					text-indent: -9999px;
					font-size: 0px;
					display: block;
				}

				/* Next Page */
				.sitetable .nav-buttons {
					padding: 16px;
					background-color: #fff;
					color: #b3b3b3;
					border-top: 1px solid #F2F2F2;
					margin-top: -1px;
				}

					.sitetable .nav-buttons:first-letter {text-transform: capitalize;}

					.sitetable .nav-buttons .nextprev {
						color: #b3b3b3;
						font-size: 14px;
					}

						.sitetable .nav-buttons .nextprev a {
							border: 0px;
							background-color: transparent;
						}

							.sitetable .nav-buttons .nextprev a:hover {
								text-decoration: underline;
								border: 0px;
								background-color: transparent;
							}

			/* Comments Page */
			.comments-page .link {
				border-radius: 2px 2px 0px 0px;
			}
				.comments-page .link .entry {border-bottom: none;padding-bottom: 15px;}

			.commentarea {
				margin-right: 316px;
			}	

				.commentarea .panestack-title {
					margin: 10px 0 0 22px;
					border-bottom: 0;
				}

					.commentarea .panestack-title .title {
						color:  #4D5763;
					}
						.panestack-title .title:first-letter {text-transform: capitalize;}

				.commentarea .menuarea {
					margin: 0 0 0 22px;
				}

					.commentarea .menuarea .spacer:nth-of-type(2) {

					}

					.commentarea .menuarea span.dropdown-title.lightdrop {color: #b3b3b3;}
					.commentarea .menuarea span.dropdown-title.lightdrop:first-letter {text-transform: capitalize;}

					.commentarea .menuarea .dropdown.lightdrop .selected {
						cursor: pointer;
						text-decoration: none;
						background-image: none;
						padding-right: 0px;
						font-weight: normal;
						color: #b3b3b3;
					}

						.commentarea .menuarea .dropdown.lightdrop .selected:hover {color: #4F8EF7;}
						.commentarea .menuarea .dropdown.lightdrop .selected:after {
							content: "▼"
						}


						.drop-choices.lightdrop {
							border: none;
							z-index: 1001;
							box-shadow: 0px 1px 3px rgba(0, 0, 0, 0.2);
						}

							.drop-choices a.choice {
								padding: 6px;
								transition: all 0.1s ease;
							}

								.drop-choices a.choice:hover {
									background-color: #4F8EF7;
									color: #fff;
								}

					.commentarea .menuarea .toggle a, .help-hoverable {
						color: #b3b3b3;
						font-weight: normal;
					}

						.commentarea .menuarea .toggle a:hover, .help-hoverable:hover {color: #4F8EF7;}

				.commentarea>.usertext {
					background-color: #FAFAFA;
					border-radius: 0px 0px 2px 2px;
					margin: -58px 0 16px 0;
					padding: 64px 16px 16px 16px;
					box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.16);
					overflow: visible;
				}

					.commentarea .usertext-edit {



					}

						.usertext-edit textarea {
							position: relative;
							z-index: 999;
						}

						.usertext .bottom-area {
							width: 500px;
						}

							.usertext .bottom-area a.reddiquette {color: #4F8EF7;}

				.gold-accent.comment-visits-box {
					margin: 0px 0px 12px 0px;
					border-radius: 2px;
				}

				.commentarea .sitetable {
					margin: 0px;
					box-shadow: none;
				}

					.commentarea .thing {
						border-radius: 2px;
						background-color: #fff;
						box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.16);
						margin: 0 0 8px 0;
						padding: 16px 16px 16px 14px;
					}

						.commentarea .child .thing {
							box-shadow: none;
							padding: 4px;
							margin: 12px 0 0 0;
						}

						.commentarea .comment .midcol {
							width: 36px;
							margin-right: 2px;
						}

					/* One stack of comments behind one parent comment */
					.commentarea .sitetable .comment {

					}
						.comment .child, .comment .showreplies {
							border-left: 1px dotted #ECECEC;
							margin-top: 0px;
						}

						/* Vote arrows */
						.comment .midcol {
							width: 24px;
							margin-right: 0px;
						}

							.comment .midcol .arrow {
								margin-left: 0px;
								margin-bottom: 4px;
							}

						.comment .entry {

						}

							.comment .entry .tagline {
								color: #b3b3b3;
								font-size: 12px;
								font-family: Arial, sans-serif;
							}

								.comment .expand {
									background-color: transparent;
									transition: all 0.15s ease;
									color: #B3B3B3;
								}


									.comment .expand:hover {
										color: #fff;
										text-decoration: none;
										background-color: #4F8EF7;
									}

								.comment .author {
									color: #4D5763;
									margin-right: 0;
									font-weight: bold;
								}

									.comment .author:hover {
										color: #4f8ef7;
										text-decoration: none;
									}

									.tagline .moderator, .green {
										color: #65B354;
										font-weight: bold;
									}

									.tagline .submitter {
										font-weight: bold;
										color: #4f8ef7;
									}


									/* RES Fixes */
									.res .thing .tagline .author.submitter {
										padding: 1px 4px;
										border-radius: 1px;
										background-color: #4F8EF7 !important;
										box-shadow: 0px 0px 0px rgba(0, 0, 0, 0);
										transition: all 0.15s ease;
									}

										.res .thing .tagline .author.submitter:hover {
											box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.2);
											background-color: #4F8EF7 !important;
										}

								.comment .score {
									font-size: inherit;
									font-weight: bold;
									color: #666;
								}

								.comment span.userattrs {
									margin-left: 4px;
								}

									.comment span.userattrs a {

									}


								/* Comment Body Text */
								.comment .usertext .md {									color: #4D5763;
								}

									.comment .usertext .md p {margin-top: 0px;}

										.md a {
											color: #4F8EF7;
										}

											.md a:visited {
												color: #7D5D8A;
											}

										.md pre {
											padding: 8px;
										}

										.md blockquote {
											border-left: 2px solid #E5E3DA;
											color: #706F6F;
										}

										.md h1, .md h2 {
											margin: 0.5em 0 0.25em 0;
											border: none;
											color: #4D5763;
										}

										.md h3 {
											color: #4D5763;
											margin: 16px 0 0 0;
										}

									/* Deleted comment */
									.usertext.grayed .usertext-body {
										margin: 4px 0;
										background-color: transparent;
										text-transform: italic;
										padding: 0;
									}


								/* Reply / Share / report */
								.comment .flat-list li a {
									color: #b3b3b3;
									font-weight: normal;
								}

									.comment .flat-list li a:hover {
										color: #4F8EF7;
										text-decoration: none;
									}

									.comment .flat-list li a[onclick*="reply"] {
										color: #4F8EF7;
										font-weight: bold;
										font-size: 11px;
									}

										.comment .flat-list li a:hover[onclick*="reply"] {

										}



								.deepthread a {color: #4F8EF7;}

				/* Sidebar stuff */
				.comments-page .side {margin-top: 312px;}

					.comments-page .side .linkinfo {
						position: absolute;
						right: 16px;
						top: 200px;
						padding: 16px;
						width: 300px;
						background-color: #fff;
						border-radius: 2px;
						box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.16);
						border: none;
					}


						.comments-page .side .linkinfo .date {color: #B3B3B3;}
							.comments-page .side .linkinfo .date:first-letter{text-transform: capitalize;}

						.comments-page .side .linkinfo .score {color: #4D5763;}

					.res.comments-page .side {margin-top: 326px;}


			/* Submission Page */
			.submit-page .side, .submit-page .content h1, #suggested-reddits {display: none;
}

			.submit-page #newlink.submit.content {
				width: 524px;
				margin: 0 auto;
			}

				.submit-page #newlink.submit.content form .spacer+.spacer {margin: 0;} 


				.submit-page #newlink.submit.content ul.tabmenu.formtab {
					padding: 0;
					border: none;
				}

					.submit-page #newlink.submit.content .tabmenu.formtab a {
						padding: 16px;
						width: 262px;
						display: inline-block;
						text-align: center;
						background-color: #fff;
						color: #4D5763;
						text-transform: uppercase;
						font-weight: bold;
						transition: all 0.25s ease;
						font-size: 16px;
						border: none;
					}

						.submit-page #newlink.submit.content .tabmenu.formtab .selected a {
							font-size: 16px;
							background-color: #516AE8;
							color: #fff;
						}

							.submit-page #newlink.submit.content .tabmenu.formtab a:hover {background-color: #e7e9f6;}
							.submit-page #newlink.submit.content .tabmenu.formtab .selected a:hover {background-color: #6379ea;}

				.submit-page .formtabs-content {border-top: 0px;padding-top: 0;}

				.submit-page .roundfield {
					padding: 16px;
					width: 524px;
					background-color: #fff;
					border-radius: 2px;
					margin-bottom: 16px;
					box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.16);
				}

					.submit-page .roundfield .title {
						color: #4D5763;
						text-transform: capitalize;
					}

				.submit-page .infobar {
					width: 524px;
					margin: 0;
					padding: 16px;
					color: #fff;
					background-color: #516AE8;
					border-radius: 0 0 2px 2px;
					border: none;
					margin-top: -12px;
					box-shadow:  0px 1px 5px rgba(0, 0, 0, 0.24);
					font-size: 0px;
				}

					.submit-page .infobar:before {
						font-size: 14px;
						content: "Please submit insightful content that allows for discussion!";}

				.content.submit .info-notice {
					background-color: #fff;
					border-radius: 2px;
					padding: 16px;
					box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.16);
					border: none;
					margin-bottom: 0px;
				}

				.submit-page #newlink.submit.content .btn {
					width: 100%;
					line-height: 41px;
					height: 42px;
					margin-top: 24px;
					background-color: #516AE8;
					border: none;
					color: #fff;
					box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.24);
					cursor: pointer;
				}

					.submit-page #newlink.submit.content .btn:hover {
						box-shadow: 0px 2px 12px rgba(0, 0, 0, 0.48);
						color: #fff;
					}

			

			/* Search Page */
			.search-page .searchpane {
				margin: 0 316px 0 0;
				background: #fff none;
				padding: 16px;
				border: none;
				border-radius: 2px 2px 0px 0px;
				box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.24);
				position: relative;
			}
				.raisedbox h4 {
					color: #B3B3B3 !important;
					font-weight: normal;
					text-transform: capitalize;
				}

				.search-page #search {
					position: inherit;
				}

					.search-page #search input[type=text] {
						box-shadow: none !important;
						font-size: 36px;
						padding: 0;
						margin: 0;
						border-radius: 0;
						border-bottom: 1px solid #E7E7E7 !important;
						margin-bottom: 9px;
					}

						.search-page #search input[type=text]:hover {
							box-shadow: none !important;
						}

					.search-page #search label {
						padding: 1em 1em 1em 1em;
						margin: 0.5em 0em;
						transition: background-color 0.1s ease;
						cursor: pointer;
						font-size: 12px;
					}
						.search-page #search label:hover {background-color: rgba(0,0,0,0.05);}

					.search-page #previoussearch p {margin-top: 1.5em;}


				.search-summary {display: none;}
				.search-page .morelink {top: 96px;}
				.search-page .side {margin-top: 148px;}



			.search-page .searchfacets {
				box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.24);
				border: none;
				padding: 16px;
				margin: 0 316px 0 0;
				background-color: #F9F9F9;
				border-radius: 0px 0px 2px 2px;
			}

				.searchfacets .title {margin: 0;}

					.searchfacets h4.title {color: #4D5763;margin: 0 0 8px 0;}
						.searchfacets h4.title:first-letter {text-transform: capitalize;}

				.searchfacets .list {margin: 0;}
				.searchfacets .facet.count {color: #B3B3B3;font-weight: normal;}
					.searchfacets .facet.count:hover {text-decoration: none;}


			.search-page .menuarea {
				border-radius: 2px 2px 0px 0px;
				border-bottom: 0px;
				margin: 16px 316px 0px 0px;
				padding :16px;
				color: #B3B3B3;
				background-color: #fff;
				box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.16);
			}

				.search-page .menuarea .dropdown.lightdrop .selected {
					text-decoration: none;
					color: #4D5763;
					font-weight: normal;
					cursor: pointer;
				}

			.search-page #noresults {

			}



			/* Wiki Page */
			.wiki-page .wikititle {
				background-color: #fff;
				padding: 9px 16px 10px 16px; 
				border-radius: 2px;
				box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.16);
				font-size: 16px;
				font-family: arial, sans-serif;
				text-transform: capitalize;
				margin: 0;
			}

			.wiki-page .pageactions {
				background-color: #fff;
				margin-left: 16px;
				border-radius: 2px;
				padding: 0px 16px;
				border: none;
				box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.16);
			}

				.wiki-page .pageactions .wikiaction {
					margin: 0;
					background-color: transparent;
					border-radius: 0px;
					padding: 10px 16px 11px 16px;
					color: #B3B3B3;
				}

					.wiki-page .pageactions .wikiaction-current {
						padding: 10px 16px 7px 16px;
						border-bottom: 4px solid #4F8EF7;
						color: #4F8EF7;
					}

						.wiki-page .pageactions .wikiaction:hover, .wiki-page .pageactions .wikiaction-current:hover {background-color: rgba(0,0,0,0.05);}

			.wiki-page .wiki-page-content {
				margin: 16px 316px 16px 0px;
				background-color: #fff;
				padding: 16px;
				border-radius: 2px;
				box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.16);
			}

				.wiki-page .wiki-page-content .wiki>.toc>ul {
					border: none;
				}

				.wiki-page .wiki-page-content .wiki.md {
					color: #4D5763;
				}
					.wiki-page .wiki-page-content .wiki.md h2 {color: #4D5763;}

					.wiki-page .wiki-page-content .wiki.md p {
						font-size: 14px;
						line-height: 1.4285714285714286em;
					}

				 	.wiki-page .wiki-page-content hr {
				 		border-style: solid;
				 		border-color: #e5e5e5;
				 	}

				 	.wiki-page .wiki-page-content em {color: #B3B3B3;}

			/* Subreddit Settings Page + Flair Page + Stylesheet Page */
			.linefield {
				background-color: #fff;
				color: #B3B3B3;
				border-radius: 2px;
				box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.16);
				margin: 0 0 8px 0;
				width: 531px;
			}

				.linefield .title {
					color: #4F8EF7;
					text-transform: capitalize;
				}

					.linefield .title:first-letter, .linefield label:first-letter {text-transform: capitalize;}
					.usertext .bottom-area a {color: #b3b3b3;}
					.usertext .bottom-area a:hover {color: #4f8ef7;}

			.pretty-form {padding-top: 24px;}
			.fancy-settings h1, .create-promotion h1 { color: rgba(255,255,255,.8); /* padding-top: 24px;margin-bottom: -18px; This was breaking stuff */}
                        .fancy-settings h1 strong {color: rgba(255,255,255,1);}

			.tabmenu {
				border-bottom: 1px solid #edeeee;
				margin-bottom: 12px;
			}

				.tabmenu li {

				}

					.tabmenu li a {
						background-color: transparent;
						color: #4D5763;
						border: none;
						font-size: 14px;
					}

					.tabmenu li.selected a {
						color: #4F8EF7;
						background-color: transparent;
						border: none;
					}


			.tabpane-content {
				border: none;
			}

				.tabpane-content .flairrow {

				}

					.tabpane-content .flairrow a.author {color: #b3b3b3;}
					.tabpane-content .tagline a {color: #4F8EF7;}

					.tabpane-content .thing .title {overflow: visible;}

			.fancy-settings .pretty-form {
				padding-top: 0px;
			}


			/* Stylesheet page */
			.stylesheet-customize-container .pretty-form {
				padding-top: 0;
				background-color: #fff;
				padding: 16px;
				margin-right: 316px;
				border-radius: 2px;
				box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.16);
				margin-bottom: 16px;
			}

				.stylesheet-customize-container .pretty-form .sheets {margin-right: 0;}

				.stylesheet-customize-container h2 {display: none;}

				.sheets .btn.right {
					background-color: transparent;
					border: none;
					box-shadow: none;
					padding: 0;
				}


				#images {
					padding: 16px;
					background-color: #fff;
					border-radius: 2px;
					box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.16);
					height: 560px;
					margin-right: 316px;
				}

					#images #image-upload {
						margin: 0em 0em 4em 0em;
					}



			/* Flairs */
			.flair {
				border: none;
				border-radius: 0px;
				font-size: 12px;
				font-family: arial, sans-serif;
				font-weight: normal;
				background-color: transparent;
				color: #B3B3B3;
				padding-left: 0px;
				margin-right: inherit;
			}

				.link .flair {font-size: 12px;}


				.flair:before {
				    margin-right: 3px;
					height: auto;
				    content: "- ";
				    margin-left: 4px;
				}

					.side .flair:before {margin-left: 0px;}



			/* Bunch of RES (Reddit Enhancement Suite) Fixes */
			.res .link .tagline a.voteWeight {background-color: transparent !important;}
			.res .thing .tagline .author.moderator {background-color: #65B354 !important;padding: 1px 4px;border-radius: 1px;}

			.res .srSep {color: rgba(255,255,255,0.45);}
			.res #RESShortcutsViewport, .res #RESShortcutsEditContainer {margin-right: 312px;}
				.res #RESShortcutsEditContainer, #RESShortcutsSort, #RESShortcutsRight, #RESShortcutsLeft, #RESShortcutsAdd, #RESShortcutsTrash {
					background-color: transparent!important;
					color: rgba(255, 255, 255, 0.45)!important;
					top: 1px !important;
				}

			.res #header-bottom-right {
				top: 1px;
				border-radius: 0px;
				height: 18px;
				padding: 0px 8px 0px 0px;
			}

				.res #userbarToggle {
					background-color: transparent;
					color: rgba(255, 255, 255, 0.45);
					border-radius: 0px;
					border: none;
				}

				.res #header-bottom-right .user .userkarma {display: none;}
				.res #header-bottom-right .user {font-size: 0px;}
				.res #header-bottom-right .user a {font-size: 11px}

				#RESAccountSwitcherIcon {
					position: relative;
					top: -4px;
				}

				.res #REScommentNavToggle {
					max-width: 98px;
					overflow: hidden;
					max-height: 15px;
					background-color: #FAFAFA;
					transition: all 0.35s ease;
				}

					.res #REScommentNavToggle:hover {
						max-width: 100%;
					}

					.res .commentarea>.usertext {
						margin-top: -74px;
						padding-top: 76px;
					}

			.res .content .RESBigEditorPop {
				background-color: rgba(0, 0, 0, 0);
				line-height: inherit;
				font-size: 11px;
				font-family: verdana,arial,sans-serif;
				box-shadow: none;
				font-weight: normal;
				color: #4D5763;
				border: none;
				padding: 0;
				height: inherit;
				margin-left: 4px;
				margin-top: 5px;
			}

			html.res-commentBoxes .comment {
				margin-left: 0 !important;
				margin-right: 0px !important;
			}

				.res .commentarea .thing {border: none !important;}


			.res .titlebox span.subscribers, .res .titlebox .users-online, .res .titlebox .number {
				top: 0px;
				left: 0px;
			}

			.res .titlebox .tagline {margin-top: 6px;}

			.res .RESshortcutside, .res .RESDashboardToggle {
				background-image: none !important;
				border: none;
				color: #4D5763;
				text-transform: uppercase;
				text-decoration: none;
				border-radius: 0px;
				padding: 4px 6px 4px 0px;
				margin: 2px 6px 2px -4px;
				text-align: left;
				width: auto;
			}

				.res .RESshortcutside:hover, .res .RESDashboardToggle:hover {
					background-color: transparent;
					color: #4F8EF7;
				}

			.res #progressIndicator {
				width: inherit;
				margin-right: 316px;
				border-radius: 0px;
				border: none;
				padding: 16px;
				margin: 16px 316px 16px 0px;
				color: #b3b3b3;
				background-color: #fff;
				height: inherit;
			}


				.res #progressIndicator h2 {
					color: #4D5763;
				}

				.res .NERPageMarker {
					border-radius: 0px;
					border: none;
					background-color: #fff;
					padding: 16px 0px;
					margin: 0px;
				}

				.res .sitetable .sitetable {margin-right: 0px;}

				.res #search #searchexpando {
					width: 300px;
					box-shadow: 0px 2px 6px rgba(0, 0, 0, 0.2);
					height: auto;
				}

					.res #search #searchexpando label {padding: 13px 0px;}

					.res #searchexpando .searchexpando-submit {display: none;}

				.res h1.hover.redditname {margin-bottom: 28px;}
				.res .titlebox .fancy-toggle-button .add, .res .fancy-toggle-button .remove {top: -78px;}
				.res .titlebox .tagline {margin-top: -14px;}
				.res .titlebox span.subscribers, .res .titlebox .users-online, .res .titlebox .number {top: -32px;}

				.res .commentarea .panestack-title {margin-top: 0px;padding-top: 12px;}

				/* Gear dropdown */
				.gearIcon {
					background: url(%%spritesheet%%) -0px -0px !important;
					position: relative;
					top: 2px;
					transition: all 0.25s ease;
				}

					#RESMainGearOverlay {
						background-color: #516ae8;
						top: 0px !important;
						height: 26px !important;
						border-radius: 0px !important;
					}

				.RESDropdownList {
					border-color: #4258ca;
					box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.24);
					margin-top: 4px;
					margin-right: 8px;
				}

					.RESDropdownList li {
						background-color: #516ae8;
						color: #fff;
						border-color: #4258ca;
						transition: all 0.15s ease;
					}

						.RESDropdownList li:first-letter {text-transform: capitalize;}

						.RESDropdownList a, .RESDropdownList a:visited { color: #fff;}

							.RESDropdownList li:hover, .RESDropdownList li a:hover {
								color: #fff;
								background-color: #667df0;
							}

						#RESSearchMenuItem {
							border: 1px solid #4258ca;
							border-radius: 1px;
							background-color: #667df0;
						}

							#RESSearchMenuItem:hover {
								background-color: #667df0;
							}

						.toggleButton {
							
						}

							.toggleButton .toggleOn, .toggleButton .toggleOff  {
								text-transform: lowercase;
							}
								/* Toggle off  */
								.moduleToggle:not(.enabled) .toggleOn, .toggleButton:not(.enabled) .toggleOn,
								.moduleToggle.enabled .toggleOff, .toggleButton.enabled .toggleOff {
									background-color: transparent;
									color: rgba(255,255,255,0.6);
									border: 1px solid #4258ca;
									transition: all 0.15s ease;
									border-radius: 2px;
								}
								/* Toggle on */
								.moduleToggle.enabled .toggleOn, .toggleButton.enabled .toggleOn,
								.moduleToggle:not(.enabled) .toggleOff, .toggleButton:not(.enabled) .toggleOff {
									background-color: #fff;
									color: #516AE8;
									font-weight: bolder;
									border: 1px solid #fff;
									transition: all 0.15s ease;
									border-radius: 2px;
								}


	/* WIP Nightmode CSS */
	.res-nightmode body {background-color: #171c1f;}

	/* Main card color */
	.res-nightmode .linklisting .link, .res-nightmode .side, .res-nightmode .listing-page .sitetable > div:nth-of-type(4n+1), 
	.res-nightmode .side .spacer > #search input, .res-nightmode .res #progressIndicator, .res-nightmode .search-page .searchpane, 
	.res-nightmode .search-page .searchfacets, .res-nightmode .search-page .menuarea, .res-nightmode .wiki-page .wiki-page-content, 
	.res-nightmode .wiki-page .wikititle, .res-nightmode .wiki-page .pageactions, .res-nightmode .side .titlebox .md h4 a, 
	.res-nightmode .wiki-page .wiki-page-content .md.wiki h4, .res-nightmode .md code, .res-nightmode .md pre, 
	.res-nightmode .stylesheet-customize-container .pretty-form, .res-nightmode #images, .res-nightmode .fancy-toggle-button .remove,
	.res-nightmode .comments-page .side .linkinfo {background-color: #21282d !important;}

	/* Secondary card color */
	.res-nightmode input:not([type="submit"]), .res-nightmode textarea, .res-nightmode .titlebox .tagline:after, .res-nightmode .commentarea>.usertext,
	.res-nightmode.res-commentBoxes .comments-page .comment, .res-nightmode.res-commentBoxes .comments-page .comment .comment .comment, 
	.res-nightmode.res-commentBoxes .comments-page .comment .comment .comment .comment .comment, 
	.res-nightmode.res-commentBoxes .comments-page .comment .comment .comment .comment .comment .comment .comment, 
	.res-nightmode.res-commentBoxes .comments-page .comment .comment .comment .comment .comment .comment .comment .comment .comment 
	{background-color: #1a2126 !important;}
	.res-nightmode .link .entry, .res-nightmode .side .titlebox .md h4 a, .res-nightmode .wiki-page .wiki-page-content .md.wiki h4, .res-nightmode .md hr,
	.res-nightmode .md code, .res-nightmode .md pre {border-color: #1a2126;}


	.res-nightmode .morelink, .res-nightmode .titlebox .fancy-toggle-button .add, .res-nightmode .morelink:after, .res-nightmode .content .infobar, .res-nightmode
	.submit-page #newlink.submit.content .tabmenu.formtab .selected a, .res-nightmode .submit-page .infobar, .res-nightmode 
	.submit-page #newlink.submit.content .btn, .res-nightmode .drop-choices a.choice:hover, .res-nightmode .linkflairlabel, .res-nightmode .fancy-toggle-button .remove:active
	.expando-button:hover, .res-nightmode .top-page .content .menuarea .dropdown.lightdrop .selected, .res-nightmode .expando-button:hover, .res-nightmode .side .titlebox .md h3 a, .res-nightmode
	.res div.RES-keyNav-activeElement, .res .res-nightmode .res div.commentarea div.RES-keyNav-activeElement.entry div.noncollapsed {background-color: #00a478}

	    /* Hover color = 10% white overlay color */
	    .res-nightmode .morelink:hover, .res-nightmode .submit-page #newlink.submit.content .tabmenu.formtab .selected a:hover, .res-nightmode
	    .side .titlebox .md h3 a:hover, .res-nightmode .titlebox .fancy-toggle-button .add:hover, .res-nightmode .titlebox .fancy-toggle-button .add:hover:after
	     {background-color: #00b987;}

	    /* Active color = 10% black overlay color */
	   .res-nightmode  .morelink:active, .res-nightmode .side .titlebox .md h3 a:active {background-color: #008a65;}


	.res-nightmode a, .res-nightmode .link .entry .buttons li a.comments, .res-nightmode .md a, .res-nightmode .titlebox .tagline a.flairselectbtn, .res-nightmode 
	.thing .title.loggedin.click, .res-nightmode .thing .title.click, .res-nightmode .thing .title.loggedin, .res-nightmode .thing .title, .res-nightmode 
	body .content .sitetable .link .title a:hover, .res-nightmode .link .domain a:hover, .res-nightmode .link .entry .buttons li a:hover, .res-nightmode 
	.link .entry .buttons li a.flairselectbtn, .res-nightmode .comment .flat-list li a[onclick*="reply"], .res-nightmode 
	.comment .flat-list li a:hover, .res-nightmode .tagline .submitter, .res-nightmode .tagline .submitter, .res-nightmode .side:after, .res-nightmode 
	.usertext .bottom-area a.reddiquette, .res-nightmode .side .titlebox .md h6 a
	 {color: #00a478;}

	 /* Nightmode misc fixes */
	 .res-nightmode .share-button .option, .res-nightmode #subscribe a, .res-nightmode .share .option, .res-nightmode .tagline a, .res-nightmode .tagline .head .author, .res-nightmode .footer a, .res-nightmode .wired a, .res-nightmode .side a, .res-nightmode .subredditbox li a, .res-nightmode .link .score.dislikes, .res-nightmode .linkcompressed .score.dislikes, .res-nightmode a[rel="tag"], .res-nightmode .dsq-help, .res-nightmode #authorInfoToolTip h3 a, .res-nightmode .RES-keyNav-activeElement .md, .res-nightmode .help-toggle .option, .res-nightmode .morecomments a, .res-nightmode .reddiquette, .res-nightmode .parent .author, .res-nightmode .parent .subreddit, .res-nightmode .comment .md p a, .res-nightmode .flair, .res-nightmode .morelink:hover a {color: #a01e5b}
	 .res-nightmode .side .titlebox, res-nightmode .side .spacer .titlebox .redditname, .res-nightmode body .content, .res-nightmode #header-bottom-right, .res-nightmode .flair, .res-nightmode .side .spacer .titlebox .redditname {background-color: transparent;}
	 .res .res-nightmode .RES-keyNav-activeElement, .res-nightmode .RES-keyNav-activeElement .usertext-body, .res-nightmode .RES-keyNav-activeElement .usertext-body .md, .res-nightmode .RES-keyNav-activeElement .usertext-body .md p, .res-nightmode .commentarea .RES-keyNav-activeElement .noncollapsed, .res-nightmode .RES-keyNav-activeElement .noncollapsed .md, .res-nightmode .RES-keyNav-activeElement .noncollapsed .md p,
	 .res-nightmode .side .md ul {background-color: transparent !important;}
	 .res-nightmode #sr-header-area, .res-nightmode #sr-more-link, .res-nightmode #RESConsoleTopBar, .res-nightmode .moduleHeader, .res-nightmode .allOptionsContainer, .res-nightmode .optionContainer {background-color: rgba(0,0,0,0.20);}
	 .res-nightmode .side .spacer .titlebox .redditname {border-color: transparent;}


	/* Experimental fadein CSS */
	.listing-page .sitetable, .search-page .sitetable, .top-page .menuarea .spacer {
		animation-name: fadein;
		animation-duration: 0.75s;
		animation-iteration-count: 1;

		-webkit-animation-name: fadein;
		-webkit-animation-duration: 0.75s;
		-webkit-animation-iteration-count: 1;
	}


			@-webkit-keyframes fadein {
			  0%   {opacity:0;transform:translateY(48px);-webkit-transform:translateY(48px);}
			  100% {opacity:1;transform:translateY(0px);-webkit-transform:translateY(0px);}
			}
		
			@-moz-keyframes fadein {
			  0%   {opacity:0;transform:translateY(48px);-webkit-transform:translateY(48px);}
			  100% {opacity:1;transform:translateY(0px);-webkit-transform:translateY(0px);}
			}
		
			@-o-keyframes fadein {
			  0%   {opacity:0;transform:translateY(48px);-webkit-transform:translateY(48px);}
			  100% {opacity:1;transform:translateY(0px);-webkit-transform:translateY(0px);}
			}
		
			@keyframes fadein {
			  0%   {opacity:0;transform:translateY(48px);-webkit-transform:translateY(48px);}
			  100% {opacity:1;transform:translateY(0px);-webkit-transform:translateY(0px);}
			}

	/* Experimental pop-in message */
	.flairselector {
		animation-name: popin;
		animation-duration: 0.5s;
		animation-iteration-count: 1;
		animation-timing-function: ease-out;

		-webkit-animation-name: popin;
		-webkit-animation-duration: 0.5s;
		-webkit-animation-iteration-count: 1;
		-webkit-animation-timing-function: ease-out;
	}

			@-webkit-keyframes popin {
			  0%   {transform:scale(0);-webkit-transform:scale(0);}
			  80%	{transform:scale(1.15);-webkit-transform:scale(1.15);}
			  100% {transform:scale(1);-webkit-transform:scale(1);}
			}
		
			@-moz-keyframes popin {
			  0%   {transform:scale(0);-webkit-transform:scale(0);}
			  80%	{transform:scale(1.15);-webkit-transform:scale(1.15);}
			  100% {transform:scale(1);-webkit-transform:scale(1);}
			}
		
			@-o-keyframes popin {
			  0%   {transform:scale(0);-webkit-transform:scale(0);}
			  80%	{transform:scale(1.15);-webkit-transform:scale(1.15);}
			  100% {transform:scale(1);-webkit-transform:scale(1);}
			}
		
			@keyframes popin {
			  0%   {transform:scale(0);-webkit-transform:scale(0);}
			  80%	{transform:scale(1.15);-webkit-transform:scale(1.15);}
			  100% {transform:scale(1);-webkit-transform:scale(1);}
			}

	/* Experimental Toast Animation */
	#mail.havemail:before {
		animation-name: toast;
		animation-duration: 8s;
		animation-iteration-count: 1;
		animation-timing-function: ease;

		-webkit-animation-name: toast;
		-webkit-animation-duration: 8s;
		-webkit-animation-iteration-count: 1;
		-webkit-animation-timing-function: ease;
	}

		#mail.havemail:hover:before {
			-webkit-animation-play-state: paused;
			 -moz-animation-play-state: paused;
			 -o-animation-play-state: paused;
			  animation-play-state: paused;
		}


		@-webkit-keyframes toast {
		  0%  	{transform:translateY(76px);	-webkit-transform:translateY(76px);	opacity: 0;}
		  20%  	{transform:translateY(76px);	-webkit-transform:translateY(76px);	opacity: 0;}
		  25%	{transform:translateY(-8px);	-webkit-transform:translateY(-8px);	opacity: 1;}
		  27%	{transform:translateY(00px);	-webkit-transform:translateY(00px);	opacity: 1;}
		  92%	{transform:translateY(00px);	-webkit-transform:translateY(00px);	opacity: 1;}
		  97%	{transform:translateY(16px);	-webkit-transform:translateY(16px);	opacity: 1;}
		  100%	{transform:translateY(76px);	-webkit-transform:translateY(76px);	opacity: 0;}
		}

		@-o-keyframes toast {
		  0%  	{transform:translateY(76px);	-webkit-transform:translateY(76px);	opacity: 0;}
		  20%  	{transform:translateY(76px);	-webkit-transform:translateY(76px);	opacity: 0;}
		  25%	{transform:translateY(-8px);	-webkit-transform:translateY(-8px);	opacity: 1;}
		  27%	{transform:translateY(00px);	-webkit-transform:translateY(00px);	opacity: 1;}
		  92%	{transform:translateY(00px);	-webkit-transform:translateY(00px);	opacity: 1;}
		  97%	{transform:translateY(16px);	-webkit-transform:translateY(16px);	opacity: 1;}
		  100%	{transform:translateY(76px);	-webkit-transform:translateY(76px);	opacity: 0;}
		}


		@-moz-keyframes toast {
		  0%  	{transform:translateY(76px);	-webkit-transform:translateY(76px);	opacity: 0;}
		  20%  	{transform:translateY(76px);	-webkit-transform:translateY(76px);	opacity: 0;}
		  25%	{transform:translateY(-8px);	-webkit-transform:translateY(-8px);	opacity: 1;}
		  27%	{transform:translateY(00px);	-webkit-transform:translateY(00px);	opacity: 1;}
		  92%	{transform:translateY(00px);	-webkit-transform:translateY(00px);	opacity: 1;}
		  97%	{transform:translateY(16px);	-webkit-transform:translateY(16px);	opacity: 1;}
		  100%	{transform:translateY(76px);	-webkit-transform:translateY(76px);	opacity: 0;}
		}


		@keyframes toast {
		  0%  	{transform:translateY(76px);	-webkit-transform:translateY(76px);	opacity: 0;}
		  20%  	{transform:translateY(76px);	-webkit-transform:translateY(76px);	opacity: 0;}
		  25%	{transform:translateY(-8px);	-webkit-transform:translateY(-8px);	opacity: 1;}
		  27%	{transform:translateY(00px);	-webkit-transform:translateY(00px);	opacity: 1;}
		  92%	{transform:translateY(00px);	-webkit-transform:translateY(00px);	opacity: 1;}
		  97%	{transform:translateY(16px);	-webkit-transform:translateY(16px);	opacity: 1;}
		  100%	{transform:translateY(76px);	-webkit-transform:translateY(76px);	opacity: 0;}
		}



		@-webkit-keyframes upvote{
		   0%   {transform:translateY(00px);	-webkit-transform:translateY(00px);  opacity:0; }
		   15%  {																	 opacity:1; }
		   80%  {																	 opacity:1;	}
		   100% {transform:translateY(-12px);	-webkit-transform:translateY(-12px); opacity:0;	}
		}

		@-moz-keyframes upvote{
		   0%   {transform:translateY(00px);	-webkit-transform:translateY(00px);  opacity:0; }
		   15%  {																	 opacity:1; }
		   80%  {																	 opacity:1;	}
		   100% {transform:translateY(-12px);	-webkit-transform:translateY(-12px); opacity:0;	}
		}

		@-o-keyframes upvote{
		   0%   {transform:translateY(00px);	-webkit-transform:translateY(00px);  opacity:0; }
		   15%  {																	 opacity:1; }
		   80%  {																	 opacity:1;	}
		   100% {transform:translateY(-12px);	-webkit-transform:translateY(-12px); opacity:0;	}
		}

		@keyframes upvote{
		   0%   {transform:translateY(00px);	-webkit-transform:translateY(00px);  opacity:0; }
		   15%  {																	 opacity:1; }
		   80%  {																	 opacity:1;	}
		   100% {transform:translateY(-12px);	-webkit-transform:translateY(-12px); opacity:0;	}
		}




/* --- Addon: Header Background Image --- */
.content:before {
width: 100%;
height: 446px; 
background: #a01e5b url(%%18theme3%%) no-repeat 33% 0; 
background-position:0 0px; 
background-size:100%;}
    @media only screen and (min-width : 1921px) {.content:before {background-size: cover;}}

        /* Add or subtract THE SAME AMOUNT ON EACH OF THESE */
.content                        {margin-top:        451px;} 
.side                           {margin-top:        555px;} 
.search-page .side              {margin-top:        503px;} 
.comments-page .side            {margin-top:        667px;}
.res .comments-page .side       {margin-top:        681px;}
.comments-page .side .linkinfo  {margin-top:        390px;} 
#search, .search-page .morelink {top:               451px;} 
.morelink                       {top:               503px;}
#header-bottom-left             {top:               365px;}

#header .tabmenu li a, .pagename a {text-shadow: 0px 1px 8px rgba(0, 0, 0, 0.5);}

/* --- End Addon --- */

/* --- Addon: Button color (Secondary Color) --- */
.titlebox .fancy-toggle-button .add, .morelink, .morelink:after, .content .infobar,
.submit-page #newlink.submit.content .tabmenu.formtab .selected a, .submit-page .infobar, 
.submit-page #newlink.submit.content .btn, .drop-choices a.choice:hover, .linkflairlabel, .fancy-toggle-button .remove:active
.expando-button:hover, .top-page .content .menuarea .dropdown.lightdrop .selected, .expando-button:hover, .side .titlebox .md h3 a,
.res div.RES-keyNav-activeElement, .res div.commentarea div.RES-keyNav-activeElement.entry div.noncollapsed {background-color: #a01e5b}

    /* Hover color = 10% white overlay color */
    .morelink:hover, .submit-page #newlink.submit.content .tabmenu.formtab .selected a:hover,
    .side .titlebox .md h3 a:hover, .titlebox .fancy-toggle-button .add:hover, .titlebox .fancy-toggle-button .add:hover:after
     {background-color: #ffffff;}

    /* Active color = 20% black overlay color */
    .morelink:active, .side .titlebox .md h3 a:active {background-color: c3c3c3;}
/* --- End Addon --- */

/* --- Addon: Link Color (Tertiary Color) - This color should be either similiar to the primary color, 
or to the secondary color. Else the page will become too busy.-- */
a, .link .entry .buttons li a.comments, .md a, .titlebox .tagline a.flairselectbtn, 
.thing .title.loggedin.click, .thing .title.click, .thing .title.loggedin, .thing .title, 
body .content .sitetable .link .title a:hover, .link .domain a:hover, .link .entry .buttons li a:hover, 
.link .entry .buttons li a.flairselectbtn, .comment .flat-list li a[onclick*="reply"], 
.comment .flat-list li a:hover, .tagline .submitter, .tagline .submitter, .side:after, 
.usertext .bottom-area a.reddiquette, .side .titlebox .md h6 a
 {color: #a01e5b;}
/* --- End Addon --- */

#header-img.submit-page {
background-image: none;
}

/*Add Image to Sidebar*/
div.side div.spacer:nth-of-type(1){
padding: 146px 0 0 !important;
background:url(%%logo%%) 
top center no-repeat;
margin-top:15px;
background-size: 300px 144px;

}
/*Link to sidebar image Add link in sidebar no punctuation*/
.side a[href*="change to url"] {
  width: 268px;
  height: 300px;
  background: url(%%logo%%) top center no-repeat;
  margin-top: 15px;
  background-size: 268px 420px;
  position: absolute;
  top: 452px;
  right: 32px;
  font-size: 0px;

}

.fancy-toggle-button .add {
    background-color: transparent !important;}


.flair {
    background: rgba(0, 0, 0, 0) url(%%flags%%) no-repeat scroll -9999px -9999px;
    border: 0 none;
    margin-left: 2px;
min-width: 16px;
	height: 11px;
	background:url(%%flags%%) no-repeat
margin-right: 5px;
   padding: 0;
position:relative;
}


.flair-ad {background-position: -16px 0}
.flair-ae {background-position: -32px 0}
.flair-af {background-position: -48px 0}
.flair-ag {background-position: -64px 0}
.flair-ai {background-position: -80px 0}
.flair-al {background-position: -96px 0}
.flair-am {background-position: -112px 0}
.flair-an {background-position: -128px 0}
.flair-ao {background-position: -144px 0}
.flair-ar {background-position: -160px 0}
.flair-as {background-position: -176px 0}
.flair-at {background-position: -192px 0}
.flair-au {background-position: -208px 0}
.flair-aw {background-position: -224px 0}
.flair-az {background-position: -240px 0}
.flair-ba {background-position: 0 -11px}
.flair-bb {background-position: -16px -11px}
.flair-bd {background-position: -32px -11px}
.flair-be {background-position: -48px -11px}
.flair-bf {background-position: -64px -11px}
.flair-bg {background-position: -80px -11px}
.flair-bh {background-position: -96px -11px}
.flair-bi {background-position: -112px -11px}
.flair-bj {background-position: -128px -11px}
.flair-bm {background-position: -144px -11px}
.flair-bn {background-position: -160px -11px}
.flair-bo {background-position: -176px -11px}
.flair-br {background-position: -192px -11px}
.flair-bs {background-position: -208px -11px}
.flair-bt {background-position: -224px -11px}
.flair-bv {background-position: -240px -11px}
.flair-bw {background-position: 0 -22px}
.flair-by {background-position: -16px -22px}
.flair-bz {background-position: -32px -22px}
.flair-ca {background-position: -48px -22px}
.flair-catalonia {background-position: -64px -22px}
.flair-cd {background-position: -80px -22px}
.flair-cf {background-position: -96px -22px}
.flair-cg {background-position: -112px -22px}
.flair-ch {background-position: -128px -22px}
.flair-ci {background-position: -144px -22px}
.flair-ck {background-position: -160px -22px}
.flair-cl {background-position: -176px -22px}
.flair-cm {background-position: -192px -22px}
.flair-cn {background-position: -208px -22px}
.flair-co {background-position: -224px -22px}
.flair-cr {background-position: -240px -22px}
.flair-cu {background-position: 0 -33px}
.flair-cv {background-position: -16px -33px}
.flair-cw {background-position: -32px -33px}
.flair-cy {background-position: -48px -33px}
.flair-cz {background-position: -64px -33px}
.flair-de {background-position: -80px -33px}
.flair-dj {background-position: -96px -33px}
.flair-dk {background-position: -112px -33px}
.flair-dm {background-position: -128px -33px}
.flair-do {background-position: -144px -33px}
.flair-dz {background-position: -160px -33px}
.flair-ec {background-position: -176px -33px}
.flair-ee {background-position: -192px -33px}
.flair-eg {background-position: -208px -33px}
.flair-eh {background-position: -224px -33px}
.flair-england {background-position: -240px -33px}
.flair-er {background-position: 0 -44px}
.flair-es {background-position: -16px -44px}
.flair-et {background-position: -32px -44px}
.flair-eu {background-position: -48px -44px}
.flair-fi {background-position: -64px -44px}
.flair-fj {background-position: -80px -44px}
.flair-fk {background-position: -96px -44px}
.flair-fm {background-position: -112px -44px}
.flair-fo {background-position: -128px -44px}
.flair-fr {background-position: -144px -44px}
.flair-ga {background-position: -160px -44px}
.flair-gb {background-position: -176px -44px}
.flair-gd {background-position: -192px -44px}
.flair-ge {background-position: -208px -44px}
.flair-gf {background-position: -224px -44px}
.flair-gg {background-position: -240px -44px}
.flair-gh {background-position: 0 -55px}
.flair-gi {background-position: -16px -55px}
.flair-gl {background-position: -32px -55px}
.flair-gm {background-position: -48px -55px}
.flair-gn {background-position: -64px -55px}
.flair-gp {background-position: -80px -55px}
.flair-gq {background-position: -96px -55px}
.flair-gr {background-position: -112px -55px}
.flair-gs {background-position: -128px -55px}
.flair-gt {background-position: -144px -55px}
.flair-gu {background-position: -160px -55px}
.flair-gw {background-position: -176px -55px}
.flair-gy {background-position: -192px -55px}
.flair-hk {background-position: -208px -55px}
.flair-hm {background-position: -224px -55px}
.flair-hn {background-position: -240px -55px}
.flair-hr {background-position: 0 -66px}
.flair-ht {background-position: -16px -66px}
.flair-hu {background-position: -32px -66px}
.flair-ic {background-position: -48px -66px}
.flair-id {background-position: -64px -66px}
.flair-ie {background-position: -80px -66px}
.flair-il {background-position: -96px -66px}
.flair-im {background-position: -112px -66px}
.flair-in {background-position: -128px -66px}
.flair-io {background-position: -144px -66px}
.flair-iq {background-position: -160px -66px}
.flair-ir {background-position: -176px -66px}
.flair-is {background-position: -192px -66px}
.flair-it {background-position: -208px -66px}
.flair-je {background-position: -224px -66px}
.flair-jm {background-position: -240px -66px}
.flair-jo {background-position: 0 -77px}
.flair-jp {background-position: -16px -77px}
.flair-ke {background-position: -32px -77px}
.flair-kg {background-position: -48px -77px}
.flair-kh {background-position: -64px -77px}
.flair-ki {background-position: -80px -77px}
.flair-km {background-position: -96px -77px}
.flair-kn {background-position: -112px -77px}
.flair-kp {background-position: -128px -77px}
.flair-kr {background-position: -144px -77px}
.flair-kurdistan {background-position: -160px -77px}
.flair-kw {background-position: -176px -77px}
.flair-ky {background-position: -192px -77px}
.flair-kz {background-position: -208px -77px}
.flair-la {background-position: -224px -77px}
.flair-lb {background-position: -240px -77px}
.flair-lc {background-position: 0 -88px}
.flair-li {background-position: -16px -88px}
.flair-lk {background-position: -32px -88px}
.flair-lr {background-position: -48px -88px}
.flair-ls {background-position: -64px -88px}
.flair-lt {background-position: -80px -88px}
.flair-lu {background-position: -96px -88px}
.flair-lv {background-position: -112px -88px}
.flair-ly {background-position: -128px -88px}
.flair-ma {background-position: -144px -88px}
.flair-mc {background-position: -160px -88px}
.flair-md {background-position: -176px -88px}
.flair-me {background-position: -192px -88px}
.flair-mg {background-position: -208px -88px}
.flair-mh {background-position: -224px -88px}
.flair-mk {background-position: -240px -88px}
.flair-ml {background-position: 0 -99px}
.flair-mm {background-position: -16px -99px}
.flair-mn {background-position: -32px -99px}
.flair-mo {background-position: -48px -99px}
.flair-mp {background-position: -64px -99px}
.flair-mq {background-position: -80px -99px}
.flair-mr {background-position: -96px -99px}
.flair-ms {background-position: -112px -99px}
.flair-mt {background-position: -128px -99px}
.flair-mu {background-position: -144px -99px}
.flair-mv {background-position: -160px -99px}
.flair-mw {background-position: -176px -99px}
.flair-mx {background-position: -192px -99px}
.flair-my {background-position: -208px -99px}
.flair-mz {background-position: -224px -99px}
.flair-na {background-position: -240px -99px}
.flair-nc {background-position: 0 -110px}
.flair-ne {background-position: -16px -110px}
.flair-nf {background-position: -32px -110px}
.flair-ng {background-position: -48px -110px}
.flair-ni {background-position: -64px -110px}
.flair-nl {background-position: -80px -110px}
.flair-no {background-position: -96px -110px}
.flair-np {background-position: -112px -110px}
.flair-nr {background-position: -128px -110px}
.flair-nu {background-position: -144px -110px}
.flair-nz {background-position: -160px -110px}
.flair-om {background-position: -176px -110px}
.flair-pa {background-position: -192px -110px}
.flair-pe {background-position: -208px -110px}
.flair-pf {background-position: -224px -110px}
.flair-pg {background-position: -240px -110px}
.flair-ph {background-position: 0 -121px}
.flair-pk {background-position: -16px -121px}
.flair-pl {background-position: -32px -121px}
.flair-pm {background-position: -48px -121px}
.flair-pn {background-position: -64px -121px}
.flair-pr {background-position: -80px -121px}
.flair-ps {background-position: -96px -121px}
.flair-pt {background-position: -112px -121px}
.flair-pw {background-position: -128px -121px}
.flair-py {background-position: -144px -121px}
.flair-qa {background-position: -160px -121px}
.flair-re {background-position: -176px -121px}
.flair-ro {background-position: -192px -121px}
.flair-rs {background-position: -208px -121px}
.flair-ru {background-position: -224px -121px}
.flair-rw {background-position: -240px -121px}
.flair-sa {background-position: 0 -132px}
.flair-sb {background-position: -16px -132px}
.flair-sc {background-position: -32px -132px}
.flair-scotland {background-position: -48px -132px}
.flair-sd {background-position: -64px -132px}
.flair-se {background-position: -80px -132px}
.flair-sg {background-position: -96px -132px}
.flair-sh {background-position: -112px -132px}
.flair-si {background-position: -128px -132px}
.flair-sk {background-position: -144px -132px}
.flair-sl {background-position: -160px -132px}
.flair-sm {background-position: -176px -132px}
.flair-sn {background-position: -192px -132px}
.flair-so {background-position: -208px -132px}
.flair-somaliland {background-position: -224px -132px}
.flair-sr {background-position: -240px -132px}
.flair-ss {background-position: 0 -143px}
.flair-st {background-position: -16px -143px}
.flair-sv {background-position: -32px -143px}
.flair-sx {background-position: -48px -143px}
.flair-sy {background-position: -64px -143px}
.flair-sz {background-position: -80px -143px}
.flair-tc {background-position: -96px -143px}
.flair-td {background-position: -112px -143px}
.flair-tf {background-position: -128px -143px}
.flair-tg {background-position: -144px -143px}
.flair-th {background-position: -160px -143px}
.flair-tibet {background-position: -176px -143px}
.flair-tj {background-position: -192px -143px}
.flair-tk {background-position: -208px -143px}
.flair-tl {background-position: -224px -143px}
.flair-tm {background-position: -240px -143px}
.flair-tn {background-position: 0 -154px}
.flair-to {background-position: -16px -154px}
.flair-tr {background-position: -32px -154px}
.flair-tt {background-position: -48px -154px}
.flair-tv {background-position: -64px -154px}
.flair-tw {background-position: -80px -154px}
.flair-tz {background-position: -96px -154px}
.flair-ua {background-position: -112px -154px}
.flair-ug {background-position: -128px -154px}
.flair-um {background-position: -144px -154px}
.flair-us {background-position: -160px -154px}
.flair-uy {background-position: -176px -154px}
.flair-uz {background-position: -192px -154px}
.flair-va {background-position: -208px -154px}
.flair-vc {background-position: -224px -154px}
.flair-ve {background-position: -240px -154px}
.flair-vg {background-position: 0 -165px}
.flair-vi {background-position: -16px -165px}
.flair-vn {background-position: -32px -165px}
.flair-vu {background-position: -48px -165px}
.flair-wales {background-position: -64px -165px}
.flair-wf {background-position: -80px -165px}
.flair-ws {background-position: -96px -165px}
.flair-xk {background-position: -112px -165px}
.flair-ye {background-position: -128px -165px}
.flair-yt {background-position: -144px -165px}
.flair-za {background-position: -160px -165px}
.flair-zanzibar {background-position: -176px -165px}
.flair-zm {background-position: -192px -165px}
.flair-zw {background-position: -208px -165px}


.flair::before {
    content: "- ";
    display: none;
    height: auto;
    margin-left: 4px;
    margin-right: 3px;
}

.comment .author {
    color: #4d5763;
    font-weight: bold;
    margin-left: 5px;
    margin-right: 0;
}

.link .entry .tagline a.author {
    margin-left: 5px;
    margin-right: inherit;
}