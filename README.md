# Double Subs
#### Watch Movies and TV Series with Double Subtitles, using MPC-HC and VSFilter | https://github.com/xDonatello/Double-Subs/
#

1) Install latest version of **MPC-HC**.<br>
   Download it from [here](https://github.com/clsid2/mpc-hc/releases) or from this repository.
#
2) Install **VSFilter (DirectVobSub)** for MPC-HC.<br>
   Download it from [here](https://nightly.mpc-hc.org/mpc-hc_apps/vsfilter/) or from this repository.
#
3) Open **MPC-HC** and configure it with **these settings** (source [here](https://github.com/clsid2/mpc-hc/issues/2497#issuecomment-1985630233)):<br>

View > Options...
- PlayBack > Output > Subtitle Renderer: Internal Subtitle Renderer
- Advanced > BlockVSFilter: FALSE
- Internal Filters > Video Decoder > Hardware Decoder to use: DXVA2 (copy-back)
- Subtitles > Misc > uncheck "Prefer external subtitles ..."
#
4) Open the **movie** with MPC-HC and select the **main subtitles** (at the bottom):<br>

Play > Subtitle Track > preferred language
#
5) Then set and select the **secondary subtitles** (at the top):<br>

Play > Filters > VSFilter (auto-loading version) > Properties...
- Main > Open... > select the .srt subtitle file
- Main > Text Settings > click on "Arial" > set 'Screen Alignment' to top
#
6) Watch your movie!