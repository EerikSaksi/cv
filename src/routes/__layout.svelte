<script>
	import '../app.postcss';
</script>

<slot />

<style global lang="css">
	@screen print {
		@page {
			margin-top: 0in;
			margin-bottom: 0in;
			margin-left: 0in;
			margin-right: 0in;
		}

		body {
			-webkit-print-color-adjust: exact !important;
			color-adjust: exact !important;
			color: black !important;
		}

		.page {
			padding: theme(spacing.16) theme(spacing.16) !important;
		}

		.initial {
			color: transparent !important;
			text-shadow: 0 0 0 #fff !important;
		}

		h1,
		h2,
		h3,
		p,
		li {
			color: black !important;
		}

		html {
			font-size: 12.288px !important;
		}
	}

	html {
		font-size: 13.176471px;
	}

	/* For Letter size */

	@screen sm {
		html {
			font-size: calc(13.176471px + (16 - 13.176471) * (100vw - 640px) / (833 - 640));
		}
	}

	@screen md {
		html {
			font-size: calc(12.288px + (16 - 12.288) * (100vw - 833px) / (1079.5 - 833));
		}
	}

	/* For A4 size */

	/* @screen sm {
html {
font-size: calc( 13.176471px + (16 - 13.176471) * (100vw - 640px) / (811 - 640) );
}
}

@screen md {
html {
font-size: calc( 12.288px + (16 - 12.288) * (100vw - 811px) / (1051 - 811) );
}
} */

	@screen lg {
		html {
			font-size: 16px;
		}
	}

	.initials-container {
		min-width: 2.31rem;
	}

	body .icon-parent::before {
		content: 'A';
		width: 0px;
		visibility: hidden;
		display: inline-block;
	}

	/* latin */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 600;
		font-display: swap;
		src: url('/fonts/FiraGO-SemiBold.latin.woff2') format('woff2');
		unicode-range: U+0000-007F, U+0080-00FF;
	}
	/* latin-ext */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 600;
		font-display: swap;
		src: url('/fonts/FiraGO-SemiBold.latin-ext.woff2') format('woff2');
		unicode-range: U+0100-017F, U+0180-024F, U+0250-02AF, U+1E00-1EFF, U+2C60-2C7F, U+A720-A7FF,
			U+AB30-AB6F;
	}
	/* cyrillic */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 600;
		font-display: swap;
		src: url('/fonts/FiraGO-SemiBold.cyrillic.woff2') format('woff2');
		unicode-range: U+0400-04FF, U+0500-052F;
	}
	/* special */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 600;
		font-display: swap;
		src: url('/fonts/FiraGO-SemiBold.special.woff2') format('woff2');
		unicode-range: U+02B0-02FF, U+0300-036F, U+1D00-1D7F, U+1D80-1DBF, U+1DC0-1DFF, U+2300-23FF,
			U+2980-29FF, U+2B00-2BFF, U+E000-F8FF, U+FB00-FB4F;
	}
	/* greek */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 600;
		font-display: swap;
		src: url('/fonts/FiraGO-SemiBold.greek.woff2') format('woff2');
		unicode-range: U+0370-03FF, U+1F00-1FFF;
	}
	/* hebrew */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 600;
		font-display: swap;
		src: url('/fonts/FiraGO-SemiBold.hebrew.woff2') format('woff2');
		unicode-range: U+0590-05FF;
	}
	/* arabic */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 600;
		font-display: swap;
		src: url('/fonts/FiraGO-SemiBold.arabic.woff2') format('woff2');
		unicode-range: U+0600-06FF, U+0750-077F, U+FB50-FDFF, U+FE70-FEFF;
	}
	/* devanagari */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 600;
		font-display: swap;
		src: url('/fonts/FiraGO-SemiBold.devanagari.woff2') format('woff2');
		unicode-range: U+0900-097F;
	}
	/* thai */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 600;
		font-display: swap;
		src: url('/fonts/FiraGO-SemiBold.thai.woff2') format('woff2');
		unicode-range: U+0E00-0E7F;
	}
	/* georgian */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 600;
		font-display: swap;
		src: url('/fonts/FiraGO-SemiBold.georgian.woff2') format('woff2');
		unicode-range: U+10A0-10FF;
	}
	/* shared */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 600;
		font-display: swap;
		src: url('/fonts/FiraGO-SemiBold.shared.woff2') format('woff2');
		unicode-range: U+2000-206F, U+2070-209F, U+20A0-20CF, U+2100-214F, U+2150-218F, U+2190-21FF,
			U+2200-22FF, U+25A0-25FF, U+2700-27BF;
	}
	/* latin */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 700;
		font-display: swap;
		src: url('/fonts/FiraGO-Bold.latin.woff2') format('woff2');
		unicode-range: U+0000-007F, U+0080-00FF;
	}
	/* latin-ext */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 700;
		font-display: swap;
		src: url('/fonts/FiraGO-Bold.latin-ext.woff2') format('woff2');
		unicode-range: U+0100-017F, U+0180-024F, U+0250-02AF, U+1E00-1EFF, U+2C60-2C7F, U+A720-A7FF,
			U+AB30-AB6F;
	}
	/* cyrillic */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 700;
		font-display: swap;
		src: url('/fonts/FiraGO-Bold.cyrillic.woff2') format('woff2');
		unicode-range: U+0400-04FF, U+0500-052F;
	}
	/* special */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 700;
		font-display: swap;
		src: url('/fonts/FiraGO-Bold.special.woff2') format('woff2');
		unicode-range: U+02B0-02FF, U+0300-036F, U+1D00-1D7F, U+1D80-1DBF, U+1DC0-1DFF, U+2300-23FF,
			U+2980-29FF, U+2B00-2BFF, U+E000-F8FF, U+FB00-FB4F;
	}
	/* greek */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 700;
		font-display: swap;
		src: url('/fonts/FiraGO-Bold.greek.woff2') format('woff2');
		unicode-range: U+0370-03FF, U+1F00-1FFF;
	}
	/* hebrew */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 700;
		font-display: swap;
		src: url('/fonts/FiraGO-Bold.hebrew.woff2') format('woff2');
		unicode-range: U+0590-05FF;
	}
	/* arabic */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 700;
		font-display: swap;
		src: url('/fonts/FiraGO-Bold.arabic.woff2') format('woff2');
		unicode-range: U+0600-06FF, U+0750-077F, U+FB50-FDFF, U+FE70-FEFF;
	}
	/* devanagari */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 700;
		font-display: swap;
		src: url('/fonts/FiraGO-Bold.devanagari.woff2') format('woff2');
		unicode-range: U+0900-097F;
	}
	/* thai */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 700;
		font-display: swap;
		src: url('/fonts/FiraGO-Bold.thai.woff2') format('woff2');
		unicode-range: U+0E00-0E7F;
	}
	/* georgian */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 700;
		font-display: swap;
		src: url('/fonts/FiraGO-Bold.georgian.woff2') format('woff2');
		unicode-range: U+10A0-10FF;
	}
	/* shared */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 700;
		font-display: swap;
		src: url('/fonts/FiraGO-Bold.shared.woff2') format('woff2');
		unicode-range: U+2000-206F, U+2070-209F, U+20A0-20CF, U+2100-214F, U+2150-218F, U+2190-21FF,
			U+2200-22FF, U+25A0-25FF, U+2700-27BF;
	}
	/* latin */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 300;
		font-display: swap;
		src: url('/fonts/FiraGO-Book.latin.woff2') format('woff2');
		unicode-range: U+0000-007F, U+0080-00FF;
	}
	/* latin-ext */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 300;
		font-display: swap;
		src: url('/fonts/FiraGO-Book.latin-ext.woff2') format('woff2');
		unicode-range: U+0100-017F, U+0180-024F, U+0250-02AF, U+1E00-1EFF, U+2C60-2C7F, U+A720-A7FF,
			U+AB30-AB6F;
	}
	/* cyrillic */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 300;
		font-display: swap;
		src: url('/fonts/FiraGO-Book.cyrillic.woff2') format('woff2');
		unicode-range: U+0400-04FF, U+0500-052F;
	}
	/* special */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 300;
		font-display: swap;
		src: url('/fonts/FiraGO-Book.special.woff2') format('woff2');
		unicode-range: U+02B0-02FF, U+0300-036F, U+1D00-1D7F, U+1D80-1DBF, U+1DC0-1DFF, U+2300-23FF,
			U+2980-29FF, U+2B00-2BFF, U+E000-F8FF, U+FB00-FB4F;
	}
	/* greek */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 300;
		font-display: swap;
		src: url('/fonts/FiraGO-Book.greek.woff2') format('woff2');
		unicode-range: U+0370-03FF, U+1F00-1FFF;
	}
	/* hebrew */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 300;
		font-display: swap;
		src: url('/fonts/FiraGO-Book.hebrew.woff2') format('woff2');
		unicode-range: U+0590-05FF;
	}
	/* arabic */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 300;
		font-display: swap;
		src: url('/fonts/FiraGO-Book.arabic.woff2') format('woff2');
		unicode-range: U+0600-06FF, U+0750-077F, U+FB50-FDFF, U+FE70-FEFF;
	}
	/* devanagari */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 300;
		font-display: swap;
		src: url('/fonts/FiraGO-Book.devanagari.woff2') format('woff2');
		unicode-range: U+0900-097F;
	}
	/* thai */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 300;
		font-display: swap;
		src: url('/fonts/FiraGO-Book.thai.woff2') format('woff2');
		unicode-range: U+0E00-0E7F;
	}
	/* georgian */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 300;
		font-display: swap;
		src: url('/fonts/FiraGO-Book.georgian.woff2') format('woff2');
		unicode-range: U+10A0-10FF;
	}
	/* shared */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 300;
		font-display: swap;
		src: url('/fonts/FiraGO-Book.shared.woff2') format('woff2');
		unicode-range: U+2000-206F, U+2070-209F, U+20A0-20CF, U+2100-214F, U+2150-218F, U+2190-21FF,
			U+2200-22FF, U+25A0-25FF, U+2700-27BF;
	}
	/* latin */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 500;
		font-display: swap;
		src: url('/fonts/FiraGO-Medium.latin.woff2') format('woff2');
		unicode-range: U+0000-007F, U+0080-00FF;
	}
	/* latin-ext */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 500;
		font-display: swap;
		src: url('/fonts/FiraGO-Medium.latin-ext.woff2') format('woff2');
		unicode-range: U+0100-017F, U+0180-024F, U+0250-02AF, U+1E00-1EFF, U+2C60-2C7F, U+A720-A7FF,
			U+AB30-AB6F;
	}
	/* cyrillic */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 500;
		font-display: swap;
		src: url('/fonts/FiraGO-Medium.cyrillic.woff2') format('woff2');
		unicode-range: U+0400-04FF, U+0500-052F;
	}
	/* special */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 500;
		font-display: swap;
		src: url('/fonts/FiraGO-Medium.special.woff2') format('woff2');
		unicode-range: U+02B0-02FF, U+0300-036F, U+1D00-1D7F, U+1D80-1DBF, U+1DC0-1DFF, U+2300-23FF,
			U+2980-29FF, U+2B00-2BFF, U+E000-F8FF, U+FB00-FB4F;
	}
	/* greek */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 500;
		font-display: swap;
		src: url('/fonts/FiraGO-Medium.greek.woff2') format('woff2');
		unicode-range: U+0370-03FF, U+1F00-1FFF;
	}
	/* hebrew */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 500;
		font-display: swap;
		src: url('/fonts/FiraGO-Medium.hebrew.woff2') format('woff2');
		unicode-range: U+0590-05FF;
	}
	/* arabic */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 500;
		font-display: swap;
		src: url('/fonts/FiraGO-Medium.arabic.woff2') format('woff2');
		unicode-range: U+0600-06FF, U+0750-077F, U+FB50-FDFF, U+FE70-FEFF;
	}
	/* devanagari */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 500;
		font-display: swap;
		src: url('/fonts/FiraGO-Medium.devanagari.woff2') format('woff2');
		unicode-range: U+0900-097F;
	}
	/* thai */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 500;
		font-display: swap;
		src: url('/fonts/FiraGO-Medium.thai.woff2') format('woff2');
		unicode-range: U+0E00-0E7F;
	}
	/* georgian */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 500;
		font-display: swap;
		src: url('/fonts/FiraGO-Medium.georgian.woff2') format('woff2');
		unicode-range: U+10A0-10FF;
	}
	/* shared */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 500;
		font-display: swap;
		src: url('/fonts/FiraGO-Medium.shared.woff2') format('woff2');
		unicode-range: U+2000-206F, U+2070-209F, U+20A0-20CF, U+2100-214F, U+2150-218F, U+2190-21FF,
			U+2200-22FF, U+25A0-25FF, U+2700-27BF;
	}
	/* latin */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 400;
		font-display: swap;
		src: url('/fonts/FiraGO-Regular.latin.woff2') format('woff2');
		unicode-range: U+0000-007F, U+0080-00FF;
	}
	/* latin-ext */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 400;
		font-display: swap;
		src: url('/fonts/FiraGO-Regular.latin-ext.woff2') format('woff2');
		unicode-range: U+0100-017F, U+0180-024F, U+0250-02AF, U+1E00-1EFF, U+2C60-2C7F, U+A720-A7FF,
			U+AB30-AB6F;
	}
	/* cyrillic */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 400;
		font-display: swap;
		src: url('/fonts/FiraGO-Regular.cyrillic.woff2') format('woff2');
		unicode-range: U+0400-04FF, U+0500-052F;
	}
	/* special */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 400;
		font-display: swap;
		src: url('/fonts/FiraGO-Regular.special.woff2') format('woff2');
		unicode-range: U+02B0-02FF, U+0300-036F, U+1D00-1D7F, U+1D80-1DBF, U+1DC0-1DFF, U+2300-23FF,
			U+2980-29FF, U+2B00-2BFF, U+E000-F8FF, U+FB00-FB4F;
	}
	/* greek */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 400;
		font-display: swap;
		src: url('/fonts/FiraGO-Regular.greek.woff2') format('woff2');
		unicode-range: U+0370-03FF, U+1F00-1FFF;
	}
	/* hebrew */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 400;
		font-display: swap;
		src: url('/fonts/FiraGO-Regular.hebrew.woff2') format('woff2');
		unicode-range: U+0590-05FF;
	}
	/* arabic */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 400;
		font-display: swap;
		src: url('/fonts/FiraGO-Regular.arabic.woff2') format('woff2');
		unicode-range: U+0600-06FF, U+0750-077F, U+FB50-FDFF, U+FE70-FEFF;
	}
	/* devanagari */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 400;
		font-display: swap;
		src: url('/fonts/FiraGO-Regular.devanagari.woff2') format('woff2');
		unicode-range: U+0900-097F;
	}
	/* thai */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 400;
		font-display: swap;
		src: url('/fonts/FiraGO-Regular.thai.woff2') format('woff2');
		unicode-range: U+0E00-0E7F;
	}
	/* georgian */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 400;
		font-display: swap;
		src: url('/fonts/FiraGO-Regular.georgian.woff2') format('woff2');
		unicode-range: U+10A0-10FF;
	}
	/* shared */
	@font-face {
		font-family: 'FiraGo';
		font-style: normal;
		font-weight: 400;
		font-display: swap;
		src: url('/fonts/FiraGO-Regular.shared.woff2') format('woff2');
		unicode-range: U+2000-206F, U+2070-209F, U+20A0-20CF, U+2100-214F, U+2150-218F, U+2190-21FF,
			U+2200-22FF, U+25A0-25FF, U+2700-27BF;
	}
</style>

