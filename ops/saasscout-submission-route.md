# SaaS Scout submission-route audit

Checked: 2026-09-09T18:44:59Z

Purpose: verify whether the public no-login submission flow can be used without supplying an email, account, payment, or private identity.

HTTP status: 200

## Server-rendered structural signals

name="viewport"
name="description"
name="turbo0-verification"
name="twelve-tools-verification"
name="fazier-verification"
name="days-launch-verification"
name="startup-fame-verification"
name="findly-tools-verification"
name="site-name"
name="site-url"
name="robots"
name="googlebot"

## Client-script endpoint signals

mber"?(r===0&&e.value===""||e.value!=r)&&(e.value=""+r):e.value!==""+r&&(e.value=""+r);else if(n==="submit"||n==="reset"){e.removeAttribute("value");return}t.hasOwnProperty("value")?Cf(e,t.type,r):t.hasOwnProperty("defaultValue")&&Cf(e,t.type,ks(t.defaultValue)),t.checked==null&&t.defa
on ug(e,t,r){if(t.hasOwnProperty("value")||t.hasOwnProperty("defaultValue")){var n=t.type;if(!(n!=="submit"&&n!=="reset"||t.value!==void 0&&t.value!==null))return;t=""+e._wrapperState.initialValue,r||t===e.value||(e.value=t),e.defaultValue=t}r=e.name,r!==""&&(e.name=""),e.defaultChecke
mpositionstart keydown keypress keyup input textInput copy cut paste click change contextmenu reset submit".split(" ");function yg(e,t){switch(e){case"focusin":case"focusout":fs=null;break;case"dragenter":case"dragleave":ms=null;break;case"mouseover":case"mouseout":ps=null;break;case"p
ncel":case"pointerdown":case"pointerup":case"ratechange":case"reset":case"resize":case"seeked":case"submit":case"touchcancel":case"touchend":case"touchstart":case"volumechange":case"change":case"selectionchange":case"textInput":case"compositionstart":case"compositionend":case"compositi
le!=="ko"?null:t.data;default:return null}}var YE={color:!0,date:!0,datetime:!0,"datetime-local":!0,email:!0,month:!0,number:!0,password:!0,range:!0,search:!0,tel:!0,text:!0,time:!0,url:!0,week:!0};function Ng(e){var t=e&&e.nodeName&&e.nodeName.toLowerCase();return t==="input"?!!YE[e.
ointerMove pointerOut pointerOver pointerUp progress rateChange reset resize seeked seeking stalled submit suspend timeUpdate touchCancel touchEnd touchStart volumeChange scroll toggle touchMove waiting wheel".split(" ");function Ds(e,t){IS.set(e,t),xo(t,[e])}for(var Ou=0;Ou<Ag.length;
ureCount:0,failureReason:null,error:null,isPaused:t.isPaused,status:"pending",variables:t.variables,submittedAt:Date.now()};case"success":return{...n,data:t.data,failureCount:0,failureReason:null,error:null,status:"success",isPaused:!1};case"error":return{...n,data:void 0,error:t.error
data:void 0,error:null,failureCount:0,failureReason:null,isPaused:!1,status:"idle",variables:void 0,submittedAt:0}}var lr,pl,$x,$4=($x=class extends Fi{constructor(t={}){super();le(this,lr);le(this,pl);this.config=t,Y(this,lr,new Map),Y(this,pl,Date.now())}build(t,r,n){const s=new L4({
lute left-4 top-1/2 transform -translate-y-1/2 h-5 w-5 text-muted-foreground"})]}),i.jsx(Ue,{href:"/submit",children:i.jsx(ae,{className:"rounded-xl px-6 py-3 font-medium shadow-sm hover:shadow-md transition-all","data-testid":"button-submit-tool",children:"Submit Tool"})})]})]})})})}f
unction WM(){const{data:e}=un({queryKey:["/api/products/count"],staleTime:18e5,gcTime:36e5});return i.jsxs("section",{className:"relative overflow-hidden min-h-[calc(100vh-5rem)] flex items-center justify-center","data-testid":
 collection of profitable SaaS tools built by indie makers. Scout innovative software solutions and submit your tool to get quality backlinks."}),i.jsxs("div",{className:"flex flex-col sm:flex-row gap-4 justify-center lg:justify-start",children:[i.jsx(ae,{variant:"outline",size:"lg",cl
d-products"]');t&&t.scrollIntoView({behavior:"smooth"})},children:"Browse Tools"}),i.jsx(Ue,{href:"/submit",children:i.jsx(ae,{size:"lg",className:"text-lg px-5 py-3 h-auto rounded-full bg-gradient-to-r from-primary to-primary/90 hover:from-primary/90 hover:to-primary transition-all du
ration-300 shadow-md hover:shadow-lg","data-testid":"button-submit-your-tool",children:"Submit Your Tool"})})]}),i.jsxs("div",{className:"mt-6 flex flex-wrap items-center justify-center lg:justify-start gap-2 text-xs text-muted-foreground",childr
gap-1 rounded-full border px-3 py-1 bg-card",children:[i.jsx("span",{children:"✅"}),"Human‑reviewed submissions"]}),i.jsxs("span",{className:"inline-flex items-center gap-1 rounded-full border px-3 py-1 bg-card",children:[i.jsx("span",{children:"🔗"}),"Quality backlink included"]}),i.jsxs("
-muted-foreground text-center lg:text-left",children:"No login needed to browse. No login needed to submit."})]}),i.jsx("div",{className:"hidden lg:block lg:w-1/3 relative",children:i.jsxs("div",{className:"relative bg-card p-6 rounded-2xl border border-border/50 shadow-sm",children:[i
-center",children:"✨"}),i.jsxs("div",{children:[i.jsx("h3",{className:"font-semibold",children:"Why submit your tool?"}),i.jsx("p",{className:"text-sm text-muted-foreground",children:"High-signal benefits for indie makers"})]})]}),i.jsxs("ul",{className:"space-y-3 text-sm",children:[i.
)]})})]})})]})}function GM({selectedCategory:e,onCategoryChange:t}){const{data:r=[]}=un({queryKey:["/api/categories"]}),n=["All",...r];return i.jsx("section",{className:"bg-card/80 backdrop-blur-sm border-y border-border/40 py-8","data-testid":"filters-section",children:i.jsx("div",{c
replace(/\s+/g,"-")}`,children:s},s))})})})})})}async function LN(e){const r=await(await ed("POST",`/api/products/${e}/upvote`)).json();return td.invalidateQueries({queryKey:["/api/products"]}),td.invalidateQueries({queryKey:["/api/products",e]}),r}async function qM(e){const r=await(a
wait ed("POST","/api/products",e)).json();return td.invalidateQueries({queryKey:["/api/products"]}),r}function $m({product:e}){const{toast:t}=hn(),r=Li();h.useEffect(()=>{typeof e.logoUrl=="string"&&e.logoUrl.trim().length>0||console.warn(`⚠️ No logoUrl defined for 
d,e.name,e.logoUrl]);const n=ro({mutationFn:LN,onMutate:async o=>{await r.cancelQueries({queryKey:["/api/products"]}),await r.cancelQueries({queryKey:["/api/products/recent"]}),await r.cancelQueries({queryKey:["/api/products",o]});const a=r.getQueryData(["/api/products"]),l=r.getQuery
Data(["/api/products/recent"]),c=r.getQueryData(["/api/products",o]);return r.setQueryData(["/api/products"],d=>d&&d.map(u=>u.id===o?{...u,upvotes:u.upvotes+1}:u)),r.setQueryData(["/api/products/recent"],d=>d&&d.map(u=>u.id===o?{...u,upvotes:u.upvotes+1}:u)),r.setQueryData(["/a
cription:"Thanks for your vote!"})},onError:(o,a,l)=>{l!=null&&l.previousProducts&&r.setQueryData(["/api/products"],l.previousProducts),l!=null&&l.previousRecentProducts&&r.setQueryData(["/api/products/recent"],l.previousRecentProducts),l!=null&&l.previousProduct&&r.setQueryData(["/ap
message||"Failed to upvote",variant:"destructive"})},onSettled:()=>{r.invalidateQueries({queryKey:["/api/products"]}),r.invalidateQueries({queryKey:["/api/products/recent"]})}}),s=o=>{o.preventDefault(),o.stopPropagation(),n.mutate(e.id)};return i.jsx(Ue,{href:`/product/${e.slug}`,chi
.useState(""),[s,o]=h.useState(100),[a,l]=h.useState("more"),{data:c=[],isLoading:d}=un({queryKey:["/api/products",e,r,s],queryFn:async()=>{const f=new URLSearchParams;e&&e!=="All"&&f.append("category",e),r&&f.append("search",r),f.append("limit",s.toString());const v=`/api/products${f
new Error(`${x.status}: ${x.statusText}`);return x.json()}}),{data:u=[],isLoading:m}=un({queryKey:["/api/products/recent"],queryFn:async()=>{const f=await fetch("/api/products/recent",{credentials:"include"});if(!f.ok)throw new Error(`${f.status}: ${f.statusText}`);return f.json()}});
lank",className:"transition-transform hover:scale-105",children:i.jsx("img",{src:"https://fazier.com/api/v1//public/badges/launch_badges.svg?badge_type=featured&theme=neutral",width:"150",alt:"Fazier badge"})}),i.jsx("a",{href:"https://dayslaunch.com",target:"_blank",rel:"noopener nor
section",{className:"bg-gradient-to-r from-primary/10 to-secondary/10 py-16","data-testid":"section-submit-cta",children:i.jsxs("div",{className:"max-w-4xl mx-auto text-center px-4 sm:px-6 lg:px-8",children:[i.jsx("h2",{className:"text-3xl font-bold text-foreground mb-4","data-testid":
"}),i.jsx("div",{className:"flex justify-center",children:i.jsx(ae,{size:"lg","data-testid":"button-submit-tool-cta",children:"Submit Your Tool"})})]})}),i.jsx("footer",{className:"bg-card border-t border-border","data-testid":"footer",children:i.jsx("div",{className:"max-w-7xl mx-auto
n:"Browse Tools"}),i.jsx("span",{className:"text-muted-foreground",children:"•"}),i.jsx("a",{href:"/submit",className:"text-muted-foreground hover:text-foreground transition-colors",children:"Submit Tool"}),i.jsx("span",{className:"text-muted-foreground",children:"•"}),i.jsx("a",{href:
toast:r}=hn(),n=Li(),[s,o]=h.useState(null),[a,l]=h.useState(0),{data:c,isLoading:d}=un({queryKey:[`/api/products/slug/${t==null?void 0:t.slug}`],enabled:!!(t!=null&&t.slug)}),u=ro({mutationFn:LN,onMutate:async b=>{const w=[`/api/products/slug/${t==null?void 0:t.slug}`];await n.cancel
Queries({queryKey:["/api/products"]}),await n.cancelQueries({queryKey:["/api/products/recent"]}),await n.cancelQueries({queryKey:w});const f=n.getQueryData(["/api/products"]),v=n.getQueryData(["/api/products/recent"]),x=n.getQueryData(w);return n.setQueryDa
ta(["/api/products"],g=>g&&g.map(y=>y.id===b?{...y,upvotes:y.upvotes+1}:y)),n.setQueryData(["/api/products/recent"],g=>g&&g.map(y=>y.id===b?{...y,upvotes:y.upvotes+1}:y)),n.setQueryData(w,g=>g&&{...g,upvotes:g.upvotes+1}),{previousProducts:f,previousRecentProducts:v,previousPro
cription:"Thanks for your vote!"})},onError:(b,w,f)=>{f!=null&&f.previousProducts&&n.setQueryData(["/api/products"],f.previousProducts),f!=null&&f.previousRecentProducts&&n.setQueryData(["/api/products/recent"],f.previousRecentProducts),f!=null&&f.previousProductDetail&&(f!=null&&f.sl
message||"Failed to upvote",variant:"destructive"})},onSettled:()=>{n.invalidateQueries({queryKey:["/api/products"]}),n.invalidateQueries({queryKey:["/api/products/recent"]}),t!=null&&t.slug&&n.invalidateQueries({queryKey:[`/api/products/slug/${t.slug}`]})}}),m=()=>{c&&u.mutate(c.id)}
$r.onSubmit,reValidateMode:$r.onChange,shouldFocusError:!0};function NO(e={}){let t={...jO,...e},r={submitCount:0,isDirty:!1,isLoading:Br(t.defaultValues),isValidating:!1,isSubmitted:!1,isSubmitting:!1,isSubmitSuccessful:!1,isValid:!1,touchedFields:{},dirtyFields:{},validatingFields:{}
,setTimeout(Ee);if(p.state.next({isSubmitted:!0,isSubmitting:!1,isSubmitSuccessful:Ht(r.errors)&&!X,submitCount:r.submitCount+1,errors:r.errors}),X)throw X},$s=(C,A={})=>{q(n,C)&&(ct(A.defaultValue)?I(C,jt(q(s,C))):(I(C,A.defaultValue),Re(s,C,jt(A.defaultValue))),A.keepTouched||pt(r.to
a.mount=!u.isValid||!!A.keepIsValid||!!A.keepDirtyValues,a.watch=!!t.shouldUnregister,p.state.next({submitCount:A.keepSubmitCount?r.submitCount:0,isDirty:G?!1:A.keepDirty?r.isDirty:!!(A.keepDefaultValues&&!es(C,s)),isSubmitted:A.keepIsSubmitted?r.isSubmitted:!1,dirtyFields:G?{}:A.keepD
ng:!1,isLoading:Br(e.defaultValues),isSubmitted:!1,isSubmitting:!1,isSubmitSuccessful:!1,isValid:!1,submitCount:0,dirtyFields:{},touchedFields:{},validatingFields:{},errors:e.errors||{},disabled:e.disabled||!1,defaultValues:Br(e.defaultValues)?void 0:e.defaultValues});t.current||(t.cur
inimum:o.value,type:"string",inclusive:!0,exact:!0,message:o.message}),n.dirty())}else if(o.kind==="email")rF.test(t.data)||(s=this._getOrReturnCtx(t,s),Q(s,{validation:"email",code:B.invalid_string,message:o.message}),n.dirty());else if(o.kind==="emoji")xf||(xf=new RegExp(nF,"u")),xf
tring,...ne.errToObj(n)})}_addCheck(t){return new Vr({...this._def,checks:[...this._def.checks,t]})}email(t){return this._addCheck({kind:"email",...ne.errToObj(t)})}url(t){return this._addCheck({kind:"url",...ne.errToObj(t)})}emoji(t){return this._addCheck({kind:"emoji",...ne.errToObj
s._def.checks.find(t=>t.kind==="duration")}get isEmail(){return!!this._def.checks.find(t=>t.kind==="email")}get isURL(){return!!this._def.checks.find(t=>t.kind==="url")}get isEmoji(){return!!this._def.checks.find(t=>t.kind==="emoji")}get isUUID(){return!!this._def.checks.find(t=>t.kin
least one tag")});async function oL(e){const t=new FormData;t.append("file",e);const r=await fetch("/api/upload",{method:"POST",body:t});if(!r.ok)throw new Error("Failed to upload file");return(await r.json()).url}async function iL(e){const t=new FormData;e.forEach(s=>t.append("files"
,s));const r=await fetch("/api/upload-multiple",{method:"POST",body:t});if(!r.ok)throw new Error("Failed to upload files");return(await r.json()).files.map(s=>s.url)}const aL=["AI","Productivity","Development","
State([]),v=k=>{n(k),k.length>0&&(d(""),y.setValue("logoUrl",""))},x=async()=>{const k=y.getValues("website");if(!k){t({title:"Website URL Required",description:"Please enter a website URL first.",variant:"destructive"});return}m(!0);try{const N=await fetch("/api/scrape-metadata",{metho
nding AI analysis request:",U);const O=await fetch("/api/ai-analyze",{method:"POST",headers:{"Content-Type":"application/json"},body:JSON.stringify(U)});if(console.log("🤖 AI Response status:",O.status),O.ok){const $=await O.json();consol
ur tool has been submitted successfully."}),e(`/product/${k.slug}`)},onError:k=>{t({title:"Error",description:k.message||"Failed to submit tool",variant:"destructive"})}}),P=async k=>{try{l(!0);let N=k.l
;r.length>0&&(N=await oL(r[0])),s.length>0&&(_=await iL(s));const D=[..._,...w];console.log("📤 Form submission - Image details:",{uploadedFiles:s.length,uploadedUrls:_.length,selectedImages:w.length,totalImages:D.length,allImageUrls:D});const U=k.tags.split(",").map($=>$.trim()).filter(Boo
"})}finally{l(!1)}};return i.jsxs("div",{className:"min-h-screen bg-background","data-testid":"page-submit-tool",children:[i.jsx(Kt,{}),i.jsxs("div",{className:"max-w-2xl mx-auto px-4 sm:px-6 lg:px-8 py-12",children:[i.jsx(Ue,{href:"/",children:i.jsxs(ae,{variant:"ghost",className:"mb-
 p-8",children:[i.jsx("h1",{className:"text-3xl font-bold text-foreground mb-2","data-testid":"text-submit-title",children:"Submit Your Tool"}),i.jsx("p",{className:"text-muted-foreground mb-8","data-testid":"text-submit-description",children:"Share your indie SaaS tool with our commun
ity. All submissions are reviewed before publishing."}),i.jsx(Il,{...y,children:i.jsxs("form",{onSubmit:y.handleSubmit(P),className:"space-y-6",children:[i.jsx(Be,{control:y.control,name:"website",re
Optional: Your X (Twitter) handle for marketing and engagement"}),i.jsx(Ve,{})]})}),i.jsx(ae,{type:"submit",size:"lg",className:"w-full",disabled:j.isPending||a,"data-testid":"button-submit-form",children:a?"Uploading files...":j.isPending?"Submitting...":"Submit Tool"}),i.jsx("div",{c
.displayName;function mL(){const{toast:e}=hn(),t=Li(),[,r]=qd(),{data:n,isLoading:s}=un({queryKey:["/api/admin/status"],queryFn:async()=>(await fetch("/api/admin/status",{credentials:"include"})).json(),retry:2,staleTime:0,cacheTime:0}),{data:o=[],isLoading:a}=un({queryKey:["/api/admi
n/submissions"],enabled:n==null?void 0:n.isAuthenticated}),l=ro({mutationFn:async b=>{await ed("POST",`/api/admin/submissions/${b}/approve`)},onSuccess:()=>{t.invalidateQueries({queryKey:["/ap
i/admin/submissions"]}),e({title:"Submission approved",description:"The tool has been approved and is now live."})},onError:()=>{e({title:"Error",description:"Failed to approve submission.",variant:
"destructive"})}}),c=ro({mutationFn:async b=>{await ed("POST",`/api/admin/submissions/${b}/reject`)},onSuccess:()=>{t.invalidateQueries({queryKey:["/api/admin/submissions"]}),e({title:"Submission rejected",description:"The submission has been rejected."})},onError
:()=>{e({title:"Error",description:"Failed to reject submission.",variant:"destructive"})}}),d=ro({mutationFn:async()=>(await fetch("/api/admin/logout",{method:"POST",credentials:"include"})).json(),onSuccess:()=>{t.clear(),r("/admin/login"),e
sName:"container mx-auto px-4 py-8",children:i.jsx("div",{className:"text-center",children:"Loading submissions..."})}):i.jsxs("div",{className:"container mx-auto px-4 py-8 max-w-4xl",children:[i.jsxs("div",{className:"mb-8 flex items-center justify-between",children:[i.jsxs("div",{childre
shboard"}),i.jsx("p",{className:"text-gray-600 dark:text-gray-400",children:"Review and manage tool submissions"})]}),i.jsxs("div",{className:"flex items-center space-x-3",children:[i.jsxs(ae,{variant:"outline",onClick:()=>r("/"),className:"flex items-center space-x-2",children:[i.jsx(oI,{
jsx("h3",{className:"text-lg font-semibold text-gray-900 dark:text-white mb-2",children:"No pending submissions"}),i.jsx("p",{className:"text-gray-600 dark:text-gray-400",children:"All submissions have been reviewed."})]})}):i.jsxs("div",{className:"space-y-6",children:[i.jsx("div",{classN

## Decision
An email-related signal exists in the public submission code. No submission was made because the sprint must not use a private contact identity without authorization.
