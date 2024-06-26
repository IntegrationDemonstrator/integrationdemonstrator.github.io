---
layout: page
title: Base Case
subtitle: Energy Balance
menubar: menu_base_case
menubar_collapsable: True
show_sidebar: false
hero_height: is-small
hero_image: ../../../img/base.jpg
left_link: /simulations/base_case/
left_link_name: Key Results
right_link: /simulations/base_case/capacities/
right_link_name: Capacities
---

First, have a look at [How to Navigate](../../../navigate) to grasp all the capabilities of the interactive results.

<div pbi-resize="powerbi" pbi-resize-src="https://app.powerbi.com/view?r=eyJrIjoiZDIzNTk2ZTItMTRlNC00Y2IyLThiNjctODcwMzM1YjcxOGM1IiwidCI6ImRkOTczZjdjLTg0ZjUtNDcwYi05MWQwLTA0M2JlZTg3ZTA3ZiIsImMiOjh9" pbi-resize-min-width="600" pbi-default-width="600px" pbi-default-height="656" pbi-resize-width="16" pbi-resize-height="9" pbi-resize-load-event="page-load" pbi-resize-header="true" pbi-resize-m-src="https://app.powerbi.com/view?r=eyJrIjoiZDIzNTk2ZTItMTRlNC00Y2IyLThiNjctODcwMzM1YjcxOGM1IiwidCI6ImRkOTczZjdjLTg0ZjUtNDcwYi05MWQwLTA0M2JlZTg3ZTA3ZiIsImMiOjh9" pbi-resize-m-width="9" pbi-resize-m-height="9" style="position: relative;"><iframe frameborder="0" allowfullscreen="true"></iframe></div><script type="text/javascript">
!function(){if("undefined"==typeof window.powerbiresizescript){window.powerbiresizescript=1;window.onmessage=function(event){var isReportPageLoadedEvent=function(event){try{if(event&&event.data&&event.data.url==='/reports/undefined/events/pageChanged'){return!0}}catch(error){return undefined}};if(isReportPageLoadedEvent(event)){var iframe=getIframeElement(event.source)
setTimeout(function(){if(iframe&&iframe.parentNode.children.length>1){switch(iframe.parentNode.getAttribute('pbi-resize-load-event')){case 'click':showElement(iframe);break;case 'page-load':case 'seconds-timeout':case 'in-view':var button=getChildByTag(iframe.parentNode,'div');setButtonState(button,'readynow');break}}},(iframe.parentNode.getAttribute('pbi-resize-delay-show')||1)*1000)}};function getChildByTag(parent,tagName){if(parent){for(var i=0;i<parent.children.length;i++){if(parent.children[i].tagName.toLowerCase()===tagName.toLowerCase()){return parent.children[i]}}}
return null}
function getIframeElement(srcWindow){var frames=document.getElementsByTagName('iframe');for(var i=0;i<frames.length;i++){if(frames[i].contentWindow===srcWindow){return frames[i]}}}
function showElement(iframe){if(!iframe){return}
var parent=iframe.parentNode;var button=getChildByTag(parent,'div');if(button){parent.removeChild(button)}
var spinner=getChildByTag(parent,'span');if(spinner){parent.removeChild(spinner)}
iframe.style.position='static';iframe.style.visibility='visible';var img=getChildByTag(parent,'img');if(img){parent.removeChild(img)}}
function setButtonState(button,state){button.setAttribute('data-state',state);var states=[{state:'waiting',text:button.getAttribute('pbi-resize-wait-txt')},{state:'loading',text:button.getAttribute('pbi-resize-load-txt')},{state:'loadingnow',text:button.getAttribute('pbi-resize-load-txt')},{state:'ready',text:button.getAttribute('pbi-resize-rdy-txt')},{state:'readynow',text:button.getAttribute('pbi-resize-load-txt')}]
var text='';for(var i=0;i<states.length;i++){if(states[i].state===state){text=states[i].text}}
var spinner=getChildByTag(button,'span');button.innerHTML=text+spinner.outerHTML;switch(state){case 'loading':button.onclick=function(){setButtonState(button,'loadingnow')}
button.parentNode.onclick=function(){setButtonState(button,'loadingnow')}
break;case 'readynow':resize();var iframe=getChildByTag(button.parentNode,'iframe');showElement(iframe)
break;case 'ready':resize();var spinner=getChildByTag(button,'span');spinner.style.display='none';button.style.width='auto';button.onclick=function(e){var iframe=getChildByTag(e.target.parentNode,'iframe');showElement(iframe)}
button.parentNode.onclick=function(e){var iframe=getChildByTag(e.target.parentNode,'iframe');showElement(iframe)}
break}}
var e=function(){for(var e=document.querySelectorAll('[pbi-resize="powerbi"]'),i=0;i<e.length;i++){e[i].style.width='100%';var actualWidth=e[i].clientWidth;var contentMinWidth=e[i].getAttribute("pbi-resize-min-width");var height=e[i].getAttribute('height');var webImg=e[i].getAttribute('pbi-resize-img');var mobileImg=e[i].getAttribute('pbi-resize-m-img')||webImg;var webWidth=e[i].getAttribute("pbi-resize-width");var webHeight=e[i].getAttribute("pbi-resize-height");var webSrc=e[i].getAttribute("pbi-resize-src");var mobileWidth=e[i].getAttribute("pbi-resize-m-width");var mobileHeight=e[i].getAttribute("pbi-resize-m-height");var mobileSrc=e[i].getAttribute("pbi-resize-m-src");var loadEvent=e[i].getAttribute('pbi-resize-load-event');var header=e[i].getAttribute('pbi-resize-header');var img=getChildByTag(e[i],'img');var iframe=getChildByTag(e[i],'iframe');var currentSrc=iframe?iframe.getAttribute('src'):null;var mobileRatio=mobileWidth/mobileHeight;var webRatio=webWidth/webHeight;var isWebSize=actualWidth>contentMinWidth;var newSrc=!(webSrc&&mobileSrc)?webSrc:(isWebSize?webSrc:mobileSrc);var resizedToWeb=((iframe&&iframe.src==mobileSrc)||(img&&img.src==mobileImg))&&isWebSize&&mobileSrc!=webSrc;var resizedToMobile=((iframe&&iframe.src==webSrc)||(img&&img.src==webImg))&&!isWebSize&&mobileSrc!=webSrc;var currentSrcIsImage=e[i].children.length>1?!0:!1;if(!currentSrc){if(iframe){iframe.style.position='absolute';iframe.style.top=0;iframe.style.left=0;iframe.style.visibility='hidden'}
if(img){img.setAttribute('src',(!isWebSize&&mobileImg)?mobileImg:webImg)}
if((!webImg&&webSrc&&isWebSize)||(!mobileImg&&mobileSrc&&!isWebSize)){iframe.setAttribute('src',(!isWebSize&&mobileSrc)?mobileSrc:webSrc);showElement(iframe);resize();break}else if((webImg&&webSrc)||(mobileImg&&mobileSrc)){var button=getChildByTag(e[i],'div');setButtonState(button,'waiting');switch(loadEvent){case 'page-load':loadIframe(iframe.parentNode,newSrc);break;case 'seconds-timeout':var timeout=parseInt(e[i].getAttribute('pbi-resize-seconds'))*1000;t=setTimeout(function(){loadIframe(iframe.parentNode,newSrc)},timeout);break;case 'in-view':if(currentSrcIsImage&&!iframe.src&&isInViewport(img)){loadIframe(iframe.parentNode,newSrc)}
window.addEventListener('scroll',function(){if(currentSrcIsImage&&!iframe.src&&isInViewport(img)){loadIframe(iframe.parentNode,newSrc)}},!1);break;case 'click':button.onclick=function(){loadIframe(iframe.parentNode,newSrc)}
e[i].firstChild.onclick=function(){loadIframe(iframe.parentNode,newSrc)}
break}}}
if((currentSrc==webImg&&!webImg&&webSrc&&isWebSize)||(currentSrc==mobileImg&&!mobileImg&&mobileSrc&&!isWebSize)){showElement(iframe)}
else if(resizedToMobile||resizedToWeb){changeCurrentSrc(e[i].children[0],isWebSize,currentSrcIsImage?webImg:webSrc,currentSrcIsImage?mobileImg:mobileSrc,newSrc)}
if(currentSrcIsImage&&((resizedToMobile&&!mobileImg&&mobileSrc)||(resizedToWeb&&!webImg&&webSrc))){showElement(iframe)}
else if(!currentSrcIsImage&&((resizedToMobile&&mobileImg&&!mobileSrc)||(resizedToWeb&&webImg&&!webSrc))){showElement(iframe)}
if(img&&img.parentNode){resizeElement(img,header,actualWidth,isWebSize,webRatio,mobileRatio,webHeight,mobileHeight)}
if(iframe){resizeElement(iframe,header,actualWidth,isWebSize,webRatio,mobileRatio,webHeight,mobileHeight)}}};function resizeElement(element,header,actualWidth,isWebSize,webRatio,mobileRatio,webHeight,mobileHeight){var warn=!1;if(mobileRatio&&mobileHeight){var pageSize=isWebSize?webRatio:mobileRatio;var pageHeight=isWebSize?webHeight:mobileHeight}
else{var pageSize=webRatio;var pageHeight=webHeight}
var p169=16.0/9.0;var p43=4.0/3.0;var heightOffset=header.toLowerCase()=="true"?36:56;if(actualWidth<569&&pageSize===p169){element.parentNode.style.width="568.88px";element.style.width="568.88px";element.style.height=320+heightOffset+"px";warn=!0}
else if(actualWidth<=437&&pageSize===p43){element.parentNode.style.width="426.66px";element.style.width="426.66px";element.style.height=320+heightOffset+"px";warn=!0}
else if(actualWidth<320||actualWidth/pageSize<320||(pageHeight<320&&pageSize!==p169&&pageSize!==p43)){var height=Math.max(actualWidth,320)/pageSize;if(height<320){element.parentNode.style.width=320*pageSize+"px";element.style.width=320*pageSize+"px";element.style.height=320+heightOffset+"px"}
else if(actualWidth<320){element.parentNode.style.width=320+"px";element.style.width=320+"px";element.style.height=height+heightOffset+"px"}
else{element.parentNode.style.width=actualWidth+"px";element.style.width=actualWidth+"px";element.style.height=height+heightOffset+"px"}
warn=!0}
else{element.parentNode.style.width="100%";element.style.width="100%";element.style.height=Math.max(element.clientWidth/pageSize,320)+heightOffset+"px"}
if(warn){console.warn("pbi-resize: requested iframe dimension is below the minimum supported dimensions. Minimum supported width is 320px. Minimum supported height is 376px. Change your Power BI report page size to ensure your content looks great when embedded in your web page or blog.")}}
document.addEventListener("DOMContentLoaded",e);window.addEventListener("resize",e);window.addEventListener("orientationchange",e);function isInViewport(e){var bounding=e.getBoundingClientRect();return(bounding.top>=0&&bounding.left>=0&&bounding.bottom<=(window.innerHeight||document.documentElement.clientHeight)&&bounding.right<=(window.innerWidth||document.documentElement.clientWidth))};function changeCurrentSrc(e,isWebSize,web,mobile,newSrc){if(web&&mobile){var iframe=e.nextElementSibling;if(e instanceof HTMLImageElement&&iframe.src&&(newSrc!=iframe.src)){iframe.setAttribute('src',newSrc);setButtonState(iframe.nextElementSibling,'loading')}
var currentSrc=isWebSize?web:mobile;e.setAttribute('src',currentSrc)}}
function resize(){if(navigator.userAgent.indexOf('MSIE')!==-1||navigator.appVersion.indexOf('Trident/')>0){var evt=document.createEvent('UIEvents');evt.initUIEvent('resize',!0,!1,window,0);window.dispatchEvent(evt)}else{window.dispatchEvent(new Event('resize'))}}
function loadIframe(parent,src){var iframe=getChildByTag(parent,'iframe');var button=getChildByTag(parent,'div');var spinner=getChildByTag(button,'span');spinner.style.display='block';var style=document.createElement('style');style.type='text/css';var keyFrames='@keyframes pbi-resize-spinner {\
                0% {\
                    transform: rotate(0deg);\
                }\
                100% {\
                    transform: rotate(360deg);\
                }\
            }';style.innerHTML=keyFrames;document.getElementsByTagName('head')[0].appendChild(style);iframe.setAttribute('src',src);iframe.setAttribute('frameborder','0');iframe.setAttribute('allowFullScreen','true');setButtonState(button,'loading')}}}();
</script>


Offshore wind, onshore wind and solar PV produce 73.3 TWh of electricity annually (the actual production is 76.4 TWh, of which 3.1 TWh is curtailed), while gas-fired combined cycles (CCGTs) produce 61.3 TWh, ensuring a low level of “Energy Not Served”. Wind and solar are intermittent and have a relatively low capacity factor (ratio between the energy effectively produced and the amount that could have been produced if an asset produced 100% of the time). In the optimum energy system, a small part of wind and solar energy is curtailed, when electricity production far exceeds demand.

<div class="table-container"  markdown="1">

|                        | Total production (TWh)* | Curtailment (TWh) | Capacity factor (%) | Usage Factor (%) | Hours of curtailment |
|------------------------|-------------------------|-------------------|---------------------|------------------|----------------------|
| Photovoltaic panels    | 28.8                    | 0.5               | 11.6                | 98.3             | 210                  |
| Onshore wind turbines  | 17.8                    | 0.5               | 22.6                | 97.4             | 405                  |
| Offshore wind turbines | 26.8                    | 2.2               | 38.2                | 92.6             | 727                  |

</div>
(* After curtailment > available in the energy system.)

Despite the capacities installed, renewable technologies never produce at their maximum capacity simultaneously. The peak combined production over an hour reaches 33.0 GW: 18.8 GW for PVs, 7.0 GW for offshore wind turbines and 7.2 GW for onshore wind turbines, taking curtailment into account.

CCGT is the only carbon-emitting dispatchable technology installed in the optimal system. CCGT plants produce 61.3 TWh of electricity, resulting in a capacity factor of 58.8 %.

PCCCs capture most of the CO<sub>2</sub> emitted by CCGTs, which consume 7.5 TWh of electricity. The remainder of the emitted CO<sub>2</sub> is compensated by using biomethane. Subtracting this consumption from electricity produced by CCGTs, results in a net production of 53.9 TWh of electricity. PCCCs are installed at 97% of the CCGT capacity.

Electricity consumption for the capture of CO<sub>2</sub> and for electrolysis reach their highest values between May and August. It follows that electricity produced by solar PVs are the main source of electricity for DAC and electrolysers and that DAC is used mainly when electricity demand is lower.

The final hydrogen demand of 77.7 TWh is mostly imported: only 1.7 TWh is produced by electrolysers in Belgium in the COASTAL cluster. Hydrogen is not used to produce methane through methanation or electricity through fuel cells.

The demand for methane is mostly used for power in CCGTs (102.2 TWh) and in final energy demand (19.6 TWh). The full potential of biomethane production in Belgium is installed (14.1 TWh) and the rest is imported (107.8 TWh). The existing storage capacity (8000 TWh) is only partly used to store 13 TWh over a year.

In total, 16.7 TWh of electricity, 76.0 TWh of hydrogen and 107.8 TWh of natural gas are imported. The next table shows the amount of energy imported and the peak value of the energy imported for each import node and neighbouring country.

<div class="table-container" markdown="1">

|                                    | Installed capacity | Total energy | Peak power   |
|------------------------------------|--------------------|--------------|--------------|
|                                    | (GW or kt/h)       | (TWh or Mt)  | (GW or kt/h) |
| INL Elec Denmark                   | 2.0                | 0.9          | 0.4          |
| INL Elec United Kingdom            | 2.4                | 4.8          | 2.4          |
| INL Elec Luxembourg                | 1.0                | 0.0          | 0.0          |
| INL Elec France                    | 8.3                | 5.5          | 5.4          |
| INL Elec Netherlands               | 5.4                | 2.2          | 1.1          |
| INL Elec Germany                   | 1.0                | 3.4          | 1.0          |
| INL H<sub>2</sub> Netherlands      | 25.7               | 76.0         | 12.3         |
| COA CH<sub>4</sub>  Norway         | 18.4               | 0.0          | 0.0          |
| COA CH<sub>4</sub>  United Kingdom | 24.5               | 0.0          | 0.0          |
| COA CH<sub>4</sub> France          | 9.4                | 78.8         | 9.4          |
| COA CH<sub>4</sub>  North Africa   | 26.8               | 0.0          | 0.0          |
| INL CH<sub>4</sub>  Germany        | 15.1               | 29.0         | 15.1         |
| INL CO<sub>2</sub> Norway          | 3.5                | 21.8         | 3.3          |

</div>

Electricity is imported from the United Kingdom, France and Germany, with 4.8, 5.6 and 3.4 TWh respectively. France and the United Kingdom are exporting nuclear power massively during winter, as solar production is low. Germany has the most renewable technologies installed, leading to high exports of energy when production exceeds demand. Small amounts of electricity are imported from Denmark, the Netherlands and Germany.
