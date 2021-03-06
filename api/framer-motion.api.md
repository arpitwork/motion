## API Report File for "framer-motion"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { CSSProperties } from 'react';
import { DetailedHTMLFactory } from 'react';
import { Easing as Easing_2 } from '@popmotion/easing';
import { ForwardRefExoticComponent } from 'react';
import { FunctionComponent } from 'react';
import { HTMLAttributes } from 'react';
import { PropsWithoutRef } from 'react';
import * as React from 'react';
import { ReactElement } from 'react';
import { ReactHTML } from 'react';
import { ReactNode } from 'react';
import { Ref } from 'react';
import { RefAttributes } from 'react';
import { RefObject } from 'react';
import { SpringProps } from 'popmotion';
import { SVGAttributes } from 'react';

// @public
export const AnimatePresence: FunctionComponent<AnimatePresenceProps>;

// @public (undocumented)
export interface AnimatePresenceProps {
    custom?: any;
    // @beta
    exitBeforeEnter?: boolean;
    initial?: boolean;
    onExitComplete?: () => void;
    // @internal
    _syncLayout?: () => void;
}

// @public
export class AnimationControls {
    // @internal
    mount(): void;
    set(definition: AnimationDefinition): void;
    // @internal
    setDefaultTransition(transition: Transition): void;
    // @internal
    setVariants(variants: Variants): void;
    // Warning: (ae-forgotten-export) The symbol "AnimationDefinition" needs to be exported by the entry point index.d.ts
    start(definition: AnimationDefinition, transitionOverride?: Transition): Promise<any>;
    stop(): void;
    // Warning: (ae-forgotten-export) The symbol "ValueAnimationControls" needs to be exported by the entry point index.d.ts
    // 
    // @internal
    subscribe(controls: ValueAnimationControls): () => boolean;
    // @internal
    unmount(): void;
    }

// Warning: (ae-internal-missing-underscore) The name "animationControls" should be prefixed with an underscore because the declaration is marked as @internal
// 
// @internal (undocumented)
export const animationControls: () => AnimationControls;

// @public (undocumented)
export interface AnimationProps {
    animate?: AnimationControls | TargetAndTransition | VariantLabels;
    // Warning: (ae-forgotten-export) The symbol "TargetResolver" needs to be exported by the entry point index.d.ts
    exit?: TargetAndTransition | VariantLabels | TargetResolver;
    // @beta
    layoutTransition?: Transition | boolean | ResolveLayoutTransition;
    positionTransition?: Transition | boolean | ResolveLayoutTransition;
    transition?: Transition;
    variants?: Variants;
}

// Warning: (ae-forgotten-export) The symbol "MotionComponentConfig" needs to be exported by the entry point index.d.ts
// Warning: (ae-internal-missing-underscore) The name "createMotionComponent" should be prefixed with an underscore because the declaration is marked as @internal
// 
// @internal (undocumented)
export const createMotionComponent: <P extends {}>({ getValueControlsConfig, loadFunctionalityComponents, renderComponent, }: MotionComponentConfig) => React.ForwardRefExoticComponent<React.PropsWithoutRef<P & MotionProps> & React.RefAttributes<Element>>;

// @public (undocumented)
export interface CustomValueType {
    // (undocumented)
    mix: (from: any, to: any) => (p: number) => number | string;
    // (undocumented)
    toValue: () => number | string;
}

// @public
export class DragControls {
    // Warning: (ae-forgotten-export) The symbol "DragControlOptions" needs to be exported by the entry point index.d.ts
    start(event: React.MouseEvent | React.TouchEvent | React.PointerEvent | MouseEvent | TouchEvent | PointerEvent, options?: DragControlOptions): void;
    // Warning: (ae-forgotten-export) The symbol "ComponentDragControls" needs to be exported by the entry point index.d.ts
    // 
    // @internal
    subscribe(controls: ComponentDragControls): () => void;
}

// @public (undocumented)
export interface DraggableProps extends DragHandlers {
    drag?: boolean | "x" | "y";
    dragConstraints?: false | {
        top?: number;
        right?: number;
        bottom?: number;
        left?: number;
    } | RefObject<Element>;
    dragControls?: DragControls;
    dragDirectionLock?: boolean;
    dragElastic?: boolean | number;
    dragListener?: boolean;
    dragMomentum?: boolean;
    dragOriginX?: MotionValue<number>;
    dragOriginY?: MotionValue<number>;
    dragPropagation?: boolean;
    // Warning: (ae-forgotten-export) The symbol "InertiaOptions" needs to be exported by the entry point index.d.ts
    dragTransition?: InertiaOptions;
    // @internal (undocumented)
    _dragTransitionControls?: AnimationControls;
    // @internal (undocumented)
    _dragValueX?: MotionValue<number>;
    // @internal (undocumented)
    _dragValueY?: MotionValue<number>;
}

// @public (undocumented)
export interface DragHandlers {
    onDirectionLock?(axis: "x" | "y"): void;
    onDrag?(event: MouseEvent | TouchEvent | PointerEvent, info: PanInfo): void;
    onDragEnd?(event: MouseEvent | TouchEvent | PointerEvent, info: PanInfo): void;
    onDragStart?(event: MouseEvent | TouchEvent | PointerEvent, info: PanInfo): void;
    onDragTransitionEnd?(): void;
}

// @public
export type EasingFunction = (v: number) => number;

// @public (undocumented)
export interface EventInfo {
    // (undocumented)
    point: Point;
}

// @public (undocumented)
export type ForwardRefComponent<T, P> = ForwardRefExoticComponent<PropsWithoutRef<P> & RefAttributes<T>>;

// @public (undocumented)
export type GestureHandlers = PanHandlers & TapHandlers & HoverHandlers;

// @public (undocumented)
export interface HoverHandlers {
    onHoverEnd?(event: MouseEvent, info: EventInfo): void;
    onHoverStart?(event: MouseEvent, info: EventInfo): void;
    whileHover?: string | TargetAndTransition;
}

// Warning: (ae-forgotten-export) The symbol "HTMLAttributesWithoutMotionProps" needs to be exported by the entry point index.d.ts
// Warning: (ae-forgotten-export) The symbol "UnwrapFactoryAttributes" needs to be exported by the entry point index.d.ts
// Warning: (ae-forgotten-export) The symbol "UnwrapFactoryElement" needs to be exported by the entry point index.d.ts
// 
// @public (undocumented)
export type HTMLMotionProps<TagName extends keyof ReactHTML> = HTMLAttributesWithoutMotionProps<UnwrapFactoryAttributes<ReactHTML[TagName]>, UnwrapFactoryElement<ReactHTML[TagName]>> & MotionProps;

// @public
export interface Inertia {
    bounceDamping?: number;
    bounceStiffness?: number;
    // @internal (undocumented)
    delay?: number;
    from?: number | string;
    max?: number;
    min?: number;
    modifyTarget?(v: number): number;
    power?: number;
    restDelta?: number;
    timeConstant?: number;
    type: "inertia";
    velocity?: number;
}

// @public
export function isValidMotionProp(key: string): boolean;

// Warning: (ae-internal-missing-underscore) The name "Keyframes" should be prefixed with an underscore because the declaration is marked as @internal
// 
// @internal
export interface Keyframes {
    // (undocumented)
    delay?: number;
    // @public
    duration?: number;
    // Warning: (ae-forgotten-export) The symbol "Easing" needs to be exported by the entry point index.d.ts
    // 
    // @public
    ease?: Easing | Easing[];
    easings?: Easing | Easing[];
    // (undocumented)
    elapsed?: number;
    // @public
    flip?: number;
    // (undocumented)
    from?: number | string;
    // @public
    loop?: number;
    // @public (undocumented)
    repeatDelay?: number;
    // @public
    times?: number[];
    // (undocumented)
    to?: number | string | ValueTarget;
    // @public
    type: "keyframes";
    values: KeyframesTarget;
    // (undocumented)
    velocity?: number;
    // @public
    yoyo?: number;
}

// @public (undocumented)
export type KeyframesTarget = ResolvedKeyframesTarget | [null, ...CustomValueType[]] | CustomValueType[];

// @public
export const motion: {
    symbol: ForwardRefComponent<SVGSymbolElement, SVGMotionProps<SVGSymbolElement>>;
    clipPath: ForwardRefComponent<SVGClipPathElement, SVGMotionProps<SVGClipPathElement>>;
    filter: ForwardRefComponent<SVGFilterElement, SVGMotionProps<SVGFilterElement>>;
    mask: ForwardRefComponent<SVGMaskElement, SVGMotionProps<SVGMaskElement>>;
    marker: ForwardRefComponent<SVGMarkerElement, SVGMotionProps<SVGMarkerElement>>;
    image: ForwardRefComponent<SVGImageElement, SVGMotionProps<SVGImageElement>>;
    text: ForwardRefComponent<SVGTextElement, SVGMotionProps<SVGTextElement>>;
    circle: ForwardRefComponent<SVGCircleElement, SVGMotionProps<SVGCircleElement>>;
    svg: ForwardRefComponent<SVGSVGElement, SVGMotionProps<SVGSVGElement>>;
    animate: ForwardRefComponent<SVGElement, SVGMotionProps<SVGElement>>;
    defs: ForwardRefComponent<SVGDefsElement, SVGMotionProps<SVGDefsElement>>;
    desc: ForwardRefComponent<SVGDescElement, SVGMotionProps<SVGDescElement>>;
    ellipse: ForwardRefComponent<SVGEllipseElement, SVGMotionProps<SVGEllipseElement>>;
    feBlend: ForwardRefComponent<SVGFEBlendElement, SVGMotionProps<SVGFEBlendElement>>;
    feColorMatrix: ForwardRefComponent<SVGFEColorMatrixElement, SVGMotionProps<SVGFEColorMatrixElement>>;
    feComponentTransfer: ForwardRefComponent<SVGFEComponentTransferElement, SVGMotionProps<SVGFEComponentTransferElement>>;
    feComposite: ForwardRefComponent<SVGFECompositeElement, SVGMotionProps<SVGFECompositeElement>>;
    feConvolveMatrix: ForwardRefComponent<SVGFEConvolveMatrixElement, SVGMotionProps<SVGFEConvolveMatrixElement>>;
    feDiffuseLighting: ForwardRefComponent<SVGFEDiffuseLightingElement, SVGMotionProps<SVGFEDiffuseLightingElement>>;
    feDisplacementMap: ForwardRefComponent<SVGFEDisplacementMapElement, SVGMotionProps<SVGFEDisplacementMapElement>>;
    feDistantLight: ForwardRefComponent<SVGFEDistantLightElement, SVGMotionProps<SVGFEDistantLightElement>>;
    feDropShadow: ForwardRefComponent<SVGFEDropShadowElement, SVGMotionProps<SVGFEDropShadowElement>>;
    feFlood: ForwardRefComponent<SVGFEFloodElement, SVGMotionProps<SVGFEFloodElement>>;
    feFuncA: ForwardRefComponent<SVGFEFuncAElement, SVGMotionProps<SVGFEFuncAElement>>;
    feFuncB: ForwardRefComponent<SVGFEFuncBElement, SVGMotionProps<SVGFEFuncBElement>>;
    feFuncG: ForwardRefComponent<SVGFEFuncGElement, SVGMotionProps<SVGFEFuncGElement>>;
    feFuncR: ForwardRefComponent<SVGFEFuncRElement, SVGMotionProps<SVGFEFuncRElement>>;
    feGaussianBlur: ForwardRefComponent<SVGFEGaussianBlurElement, SVGMotionProps<SVGFEGaussianBlurElement>>;
    feImage: ForwardRefComponent<SVGFEImageElement, SVGMotionProps<SVGFEImageElement>>;
    feMerge: ForwardRefComponent<SVGFEMergeElement, SVGMotionProps<SVGFEMergeElement>>;
    feMergeNode: ForwardRefComponent<SVGFEMergeNodeElement, SVGMotionProps<SVGFEMergeNodeElement>>;
    feMorphology: ForwardRefComponent<SVGFEMorphologyElement, SVGMotionProps<SVGFEMorphologyElement>>;
    feOffset: ForwardRefComponent<SVGFEOffsetElement, SVGMotionProps<SVGFEOffsetElement>>;
    fePointLight: ForwardRefComponent<SVGFEPointLightElement, SVGMotionProps<SVGFEPointLightElement>>;
    feSpecularLighting: ForwardRefComponent<SVGFESpecularLightingElement, SVGMotionProps<SVGFESpecularLightingElement>>;
    feSpotLight: ForwardRefComponent<SVGFESpotLightElement, SVGMotionProps<SVGFESpotLightElement>>;
    feTile: ForwardRefComponent<SVGFETileElement, SVGMotionProps<SVGFETileElement>>;
    feTurbulence: ForwardRefComponent<SVGFETurbulenceElement, SVGMotionProps<SVGFETurbulenceElement>>;
    foreignObject: ForwardRefComponent<SVGForeignObjectElement, SVGMotionProps<SVGForeignObjectElement>>;
    g: ForwardRefComponent<SVGGElement, SVGMotionProps<SVGGElement>>;
    line: ForwardRefComponent<SVGLineElement, SVGMotionProps<SVGLineElement>>;
    linearGradient: ForwardRefComponent<SVGLinearGradientElement, SVGMotionProps<SVGLinearGradientElement>>;
    metadata: ForwardRefComponent<SVGMetadataElement, SVGMotionProps<SVGMetadataElement>>;
    path: ForwardRefComponent<SVGPathElement, SVGMotionProps<SVGPathElement>>;
    pattern: ForwardRefComponent<SVGPatternElement, SVGMotionProps<SVGPatternElement>>;
    polygon: ForwardRefComponent<SVGPolygonElement, SVGMotionProps<SVGPolygonElement>>;
    polyline: ForwardRefComponent<SVGPolylineElement, SVGMotionProps<SVGPolylineElement>>;
    radialGradient: ForwardRefComponent<SVGRadialGradientElement, SVGMotionProps<SVGRadialGradientElement>>;
    rect: ForwardRefComponent<SVGRectElement, SVGMotionProps<SVGRectElement>>;
    stop: ForwardRefComponent<SVGStopElement, SVGMotionProps<SVGStopElement>>;
    switch: ForwardRefComponent<SVGSwitchElement, SVGMotionProps<SVGSwitchElement>>;
    textPath: ForwardRefComponent<SVGTextPathElement, SVGMotionProps<SVGTextPathElement>>;
    tspan: ForwardRefComponent<SVGTSpanElement, SVGMotionProps<SVGTSpanElement>>;
    use: ForwardRefComponent<SVGUseElement, SVGMotionProps<SVGUseElement>>;
    view: ForwardRefComponent<SVGViewElement, SVGMotionProps<SVGViewElement>>;
    object: ForwardRefComponent<HTMLObjectElement, HTMLMotionProps<"object">>;
    style: ForwardRefComponent<HTMLStyleElement, HTMLMotionProps<"style">>;
    progress: ForwardRefComponent<HTMLProgressElement, HTMLMotionProps<"progress">>;
    ruby: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    table: ForwardRefComponent<HTMLTableElement, HTMLMotionProps<"table">>;
    small: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    sub: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    embed: ForwardRefComponent<HTMLEmbedElement, HTMLMotionProps<"embed">>;
    pre: ForwardRefComponent<HTMLPreElement, HTMLMotionProps<"pre">>;
    caption: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    menu: ForwardRefComponent<HTMLElement, HTMLMotionProps<"menu">>;
    button: ForwardRefComponent<HTMLButtonElement, HTMLMotionProps<"button">>;
    menuitem: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    meter: ForwardRefComponent<HTMLElement, HTMLMotionProps<"meter">>;
    textarea: ForwardRefComponent<HTMLTextAreaElement, HTMLMotionProps<"textarea">>;
    time: ForwardRefComponent<HTMLElement, HTMLMotionProps<"time">>;
    link: ForwardRefComponent<HTMLLinkElement, HTMLMotionProps<"link">>;
    dialog: ForwardRefComponent<HTMLDialogElement, HTMLMotionProps<"dialog">>;
    a: ForwardRefComponent<HTMLAnchorElement, HTMLMotionProps<"a">>;
    abbr: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    address: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    area: ForwardRefComponent<HTMLAreaElement, HTMLMotionProps<"area">>;
    article: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    aside: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    audio: ForwardRefComponent<HTMLAudioElement, HTMLMotionProps<"audio">>;
    b: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    base: ForwardRefComponent<HTMLBaseElement, HTMLMotionProps<"base">>;
    bdi: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    bdo: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    big: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    blockquote: ForwardRefComponent<HTMLElement, HTMLMotionProps<"blockquote">>;
    body: ForwardRefComponent<HTMLBodyElement, HTMLMotionProps<"body">>;
    br: ForwardRefComponent<HTMLBRElement, HTMLMotionProps<"br">>;
    canvas: ForwardRefComponent<HTMLCanvasElement, HTMLMotionProps<"canvas">>;
    cite: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    code: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    col: ForwardRefComponent<HTMLTableColElement, HTMLMotionProps<"col">>;
    colgroup: ForwardRefComponent<HTMLTableColElement, HTMLMotionProps<"colgroup">>;
    data: ForwardRefComponent<HTMLDataElement, HTMLMotionProps<"data">>;
    datalist: ForwardRefComponent<HTMLDataListElement, HTMLMotionProps<"datalist">>;
    dd: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    del: ForwardRefComponent<HTMLElement, HTMLMotionProps<"del">>;
    details: ForwardRefComponent<HTMLElement, HTMLMotionProps<"details">>;
    dfn: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    div: ForwardRefComponent<HTMLDivElement, HTMLMotionProps<"div">>;
    dl: ForwardRefComponent<HTMLDListElement, HTMLMotionProps<"dl">>;
    dt: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    em: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    fieldset: ForwardRefComponent<HTMLFieldSetElement, HTMLMotionProps<"fieldset">>;
    figcaption: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    figure: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    footer: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    form: ForwardRefComponent<HTMLFormElement, HTMLMotionProps<"form">>;
    h1: ForwardRefComponent<HTMLHeadingElement, HTMLMotionProps<"h1">>;
    h2: ForwardRefComponent<HTMLHeadingElement, HTMLMotionProps<"h1">>;
    h3: ForwardRefComponent<HTMLHeadingElement, HTMLMotionProps<"h1">>;
    h4: ForwardRefComponent<HTMLHeadingElement, HTMLMotionProps<"h1">>;
    h5: ForwardRefComponent<HTMLHeadingElement, HTMLMotionProps<"h1">>;
    h6: ForwardRefComponent<HTMLHeadingElement, HTMLMotionProps<"h1">>;
    head: ForwardRefComponent<HTMLHeadElement, HTMLMotionProps<"head">>;
    header: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    hgroup: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    hr: ForwardRefComponent<HTMLHRElement, HTMLMotionProps<"hr">>;
    html: ForwardRefComponent<HTMLHtmlElement, HTMLMotionProps<"html">>;
    i: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    iframe: ForwardRefComponent<HTMLIFrameElement, HTMLMotionProps<"iframe">>;
    img: ForwardRefComponent<HTMLImageElement, HTMLMotionProps<"img">>;
    input: ForwardRefComponent<HTMLInputElement, HTMLMotionProps<"input">>;
    ins: ForwardRefComponent<HTMLModElement, HTMLMotionProps<"ins">>;
    kbd: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    keygen: ForwardRefComponent<HTMLElement, HTMLMotionProps<"keygen">>;
    label: ForwardRefComponent<HTMLLabelElement, HTMLMotionProps<"label">>;
    legend: ForwardRefComponent<HTMLLegendElement, HTMLMotionProps<"legend">>;
    li: ForwardRefComponent<HTMLLIElement, HTMLMotionProps<"li">>;
    main: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    map: ForwardRefComponent<HTMLMapElement, HTMLMotionProps<"map">>;
    mark: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    meta: ForwardRefComponent<HTMLMetaElement, HTMLMotionProps<"meta">>;
    nav: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    noscript: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    ol: ForwardRefComponent<HTMLOListElement, HTMLMotionProps<"ol">>;
    optgroup: ForwardRefComponent<HTMLOptGroupElement, HTMLMotionProps<"optgroup">>;
    option: ForwardRefComponent<HTMLOptionElement, HTMLMotionProps<"option">>;
    output: ForwardRefComponent<HTMLElement, HTMLMotionProps<"output">>;
    p: ForwardRefComponent<HTMLParagraphElement, HTMLMotionProps<"p">>;
    param: ForwardRefComponent<HTMLParamElement, HTMLMotionProps<"param">>;
    picture: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    q: ForwardRefComponent<HTMLQuoteElement, HTMLMotionProps<"q">>;
    rp: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    rt: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    s: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    samp: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    script: ForwardRefComponent<HTMLScriptElement, HTMLMotionProps<"script">>;
    section: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    select: ForwardRefComponent<HTMLSelectElement, HTMLMotionProps<"select">>;
    source: ForwardRefComponent<HTMLSourceElement, HTMLMotionProps<"source">>;
    span: ForwardRefComponent<HTMLSpanElement, HTMLMotionProps<"span">>;
    strong: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    summary: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    sup: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    tbody: ForwardRefComponent<HTMLTableSectionElement, HTMLMotionProps<"tbody">>;
    td: ForwardRefComponent<HTMLTableDataCellElement, HTMLMotionProps<"td">>;
    tfoot: ForwardRefComponent<HTMLTableSectionElement, HTMLMotionProps<"tbody">>;
    th: ForwardRefComponent<HTMLTableHeaderCellElement, HTMLMotionProps<"th">>;
    thead: ForwardRefComponent<HTMLTableSectionElement, HTMLMotionProps<"tbody">>;
    title: ForwardRefComponent<HTMLTitleElement, HTMLMotionProps<"title">>;
    tr: ForwardRefComponent<HTMLTableRowElement, HTMLMotionProps<"tr">>;
    track: ForwardRefComponent<HTMLTrackElement, HTMLMotionProps<"track">>;
    u: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    ul: ForwardRefComponent<HTMLUListElement, HTMLMotionProps<"ul">>;
    var: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    video: ForwardRefComponent<HTMLVideoElement, HTMLMotionProps<"video">>;
    wbr: ForwardRefComponent<HTMLElement, HTMLMotionProps<"ruby">>;
    webview: ForwardRefComponent<HTMLWebViewElement, HTMLMotionProps<"webview">>;
    custom: <Props>(Component: string | React.ComponentClass<Props, any> | React.FunctionComponent<Props>) => React.ForwardRefExoticComponent<React.PropsWithoutRef<Props & MotionProps> & React.RefAttributes<Element>>;
};

// @public (undocumented)
export interface MotionAdvancedProps {
    custom?: any;
    inherit?: boolean;
    // @internal
    static?: boolean;
}

// @public (undocumented)
export interface MotionCallbacks {
    onAnimationComplete?(): void;
    onAnimationStart?(): void;
    onUpdate?(latest: {
        [key: string]: string | number;
    }): void;
}

// Warning: (ae-forgotten-export) The symbol "MotionContextProps" needs to be exported by the entry point index.d.ts
// Warning: (ae-internal-missing-underscore) The name "MotionContext" should be prefixed with an underscore because the declaration is marked as @internal
// 
// @internal (undocumented)
export const MotionContext: React.Context<MotionContextProps>;

// Warning: (ae-forgotten-export) The symbol "MotionPluginsContext" needs to be exported by the entry point index.d.ts
// Warning: (ae-internal-missing-underscore) The name "MotionPluginContext" should be prefixed with an underscore because the declaration is marked as @internal
// 
// @internal (undocumented)
export const MotionPluginContext: React.Context<MotionPluginsContext>;

// Warning: (ae-forgotten-export) The symbol "MotionPluginProps" needs to be exported by the entry point index.d.ts
// Warning: (ae-internal-missing-underscore) The name "MotionPlugins" should be prefixed with an underscore because the declaration is marked as @internal
// 
// @internal (undocumented)
export function MotionPlugins({ children, ...props }: MotionPluginProps): JSX.Element;

// @public
export interface MotionProps extends AnimationProps, MotionCallbacks, GestureHandlers, DraggableProps, MotionAdvancedProps {
    // Warning: (ae-forgotten-export) The symbol "Target" needs to be exported by the entry point index.d.ts
    initial?: boolean | Target | VariantLabels;
    style?: MotionStyle;
    // Warning: (ae-forgotten-export) The symbol "TransformProperties" needs to be exported by the entry point index.d.ts
    transformTemplate?(transform: TransformProperties, generatedTransform: string): string;
    // @internal
    transformValues?<V extends any>(values: V): V;
}

// Warning: (ae-forgotten-export) The symbol "MotionCSS" needs to be exported by the entry point index.d.ts
// Warning: (ae-forgotten-export) The symbol "MakeMotion" needs to be exported by the entry point index.d.ts
// Warning: (ae-forgotten-export) The symbol "SVGPathProperties" needs to be exported by the entry point index.d.ts
// Warning: (ae-forgotten-export) The symbol "MakeCustomValueType" needs to be exported by the entry point index.d.ts
// Warning: (ae-forgotten-export) The symbol "CustomStyles" needs to be exported by the entry point index.d.ts
// 
// @public (undocumented)
export type MotionStyle = MotionCSS & MotionTransform & MakeMotion<SVGPathProperties> & MakeCustomValueType<CustomStyles>;

// @public (undocumented)
export type MotionTransform = MakeMotion<TransformProperties>;

// @public
export class MotionValue<V = any> {
    // Warning: (ae-forgotten-export) The symbol "Config" needs to be exported by the entry point index.d.ts
    // 
    // @internal
    constructor(init: V, { transformer, parent }?: Config<V>);
    // @internal
    addChild(config?: Config<V>): MotionValue<V>;
    // @internal
    attach(passiveEffect: PassiveEffect<V>): void;
    destroy(): void;
    get(): V;
    getVelocity(): number;
    isAnimating(): boolean;
    onChange(subscription: Subscriber<V>): () => void;
    // @internal
    onRenderRequest(subscription: Subscriber<V>): () => boolean;
    // @internal
    removeChild(child: MotionValue): void;
    set(v: V, render?: boolean): void;
    // Warning: (ae-forgotten-export) The symbol "StartAnimation" needs to be exported by the entry point index.d.ts
    // 
    // @internal
    start(animation: StartAnimation): Promise<void>;
    stop(): void;
    // (undocumented)
    updateAndNotify: (v: V, render?: boolean) => void;
    // @internal
    updateSubscribers?: Set<Subscriber<V>>;
    }

// Warning: (ae-internal-missing-underscore) The name "motionValue" should be prefixed with an underscore because the declaration is marked as @internal
// 
// @internal (undocumented)
export function motionValue<V>(init: V, opts?: Config<V>): MotionValue<V>;

// @public (undocumented)
export interface None {
    // @internal (undocumented)
    delay?: number;
    // @internal (undocumented)
    from?: number | string;
    type: false;
    // @internal (undocumented)
    velocity?: number;
}

// @public
export interface Orchestration {
    delay?: number;
    delayChildren?: number;
    staggerChildren?: number;
    staggerDirection?: number;
    when?: false | "beforeChildren" | "afterChildren" | string;
}

// @public (undocumented)
export interface PanHandlers {
    onPan?(event: MouseEvent | TouchEvent | PointerEvent, info: PanInfo): void;
    onPanEnd?(event: MouseEvent | TouchEvent | PointerEvent, info: PanInfo): void;
    onPanSessionStart?(event: MouseEvent | TouchEvent | PointerEvent, info: EventInfo): void;
    onPanStart?(event: MouseEvent | TouchEvent | PointerEvent, info: PanInfo): void;
}

// @public
export interface PanInfo {
    delta: Point;
    offset: Point;
    point: Point;
    velocity: Point;
}

// @public (undocumented)
export type PassiveEffect<T> = (v: T, safeSetter: (v: T) => void) => void;

// @public (undocumented)
export interface Point {
    // (undocumented)
    x: number;
    // (undocumented)
    y: number;
}

// @public (undocumented)
export namespace Point {
    const // @beta (undocumented)
    subtract: (a: Point, b: Point) => Point;
    const // @beta (undocumented)
    relativeTo: (idOrElem: string | HTMLElement) => ({ x, y }: Point) => Point | undefined;
}

// Warning: (ae-forgotten-export) The symbol "Props" needs to be exported by the entry point index.d.ts
// Warning: (ae-internal-missing-underscore) The name "ReducedMotion" should be prefixed with an underscore because the declaration is marked as @internal
// 
// @internal
export function ReducedMotion({ children, enabled }: Props): JSX.Element;

// @public (undocumented)
export interface RelayoutInfo {
    // (undocumented)
    delta: {
        x: number;
        y: number;
        width: number;
        height: number;
    };
}

// @public (undocumented)
export type ResolvedKeyframesTarget = [null, ...number[]] | number[] | [null, ...string[]] | string[];

// @public (undocumented)
export type ResolvedSingleTarget = string | number;

// @public (undocumented)
export type ResolvedValueTarget = ResolvedSingleTarget | ResolvedKeyframesTarget;

// @public (undocumented)
export type ResolveLayoutTransition = (info: RelayoutInfo) => Transition | boolean;

// @public (undocumented)
export interface ScrollMotionValues {
    // (undocumented)
    scrollX: MotionValue<number>;
    // (undocumented)
    scrollXProgress: MotionValue<number>;
    // (undocumented)
    scrollY: MotionValue<number>;
    // (undocumented)
    scrollYProgress: MotionValue<number>;
}

// @public (undocumented)
export type SingleTarget = ResolvedSingleTarget | CustomValueType;

// @public
export interface Spring {
    damping?: number;
    // @internal (undocumented)
    delay?: number;
    from?: number | string;
    mass?: number;
    restDelta?: number;
    restSpeed?: number;
    stiffness?: number;
    // @internal (undocumented)
    to?: number | string | ValueTarget;
    type: "spring";
    velocity?: number;
}

// @public (undocumented)
export type Subscriber<T> = (v: T) => void;

// Warning: (ae-forgotten-export) The symbol "SVGAttributesWithoutMotionProps" needs to be exported by the entry point index.d.ts
// 
// @public
export type SVGAttributesAsMotionValues<T> = MakeMotion<SVGAttributesWithoutMotionProps<T>>;

// Warning: (ae-forgotten-export) The symbol "Omit" needs to be exported by the entry point index.d.ts
// 
// @public (undocumented)
export interface SVGMotionProps<T> extends SVGAttributesAsMotionValues<T>, Omit<MotionProps, "positionTransition"> {
}

// @public (undocumented)
export interface TapHandlers {
    onTap?(event: MouseEvent | TouchEvent | PointerEvent, info: TapInfo): void;
    onTapCancel?(event: MouseEvent | TouchEvent | PointerEvent, info: TapInfo): void;
    onTapStart?(event: MouseEvent | TouchEvent | PointerEvent, info: TapInfo): void;
    whileTap?: string | TargetAndTransition;
}

// @public
export interface TapInfo {
    point: Point;
}

// Warning: (ae-forgotten-export) The symbol "TargetWithKeyframes" needs to be exported by the entry point index.d.ts
// 
// @public
export type TargetAndTransition = TargetWithKeyframes & {
    transition?: Transition;
    transitionEnd?: Target;
};

// Warning: (ae-forgotten-export) The symbol "TransformOptions" needs to be exported by the entry point index.d.ts
// 
// @public
export function transform<T>(inputValue: number, inputRange: number[], outputRange: T[], options?: TransformOptions<T>): T;

// @public
export function transform<T>(inputRange: number[], outputRange: T[], options?: TransformOptions<T>): (inputValue: number) => T;

// Warning: (ae-forgotten-export) The symbol "TransitionDefinition" needs to be exported by the entry point index.d.ts
// Warning: (ae-forgotten-export) The symbol "TransitionMap" needs to be exported by the entry point index.d.ts
// 
// @public
export type Transition = (Orchestration & TransitionDefinition) | (Orchestration & TransitionMap);

// @public
export interface Tween {
    // @internal (undocumented)
    delay?: number;
    duration?: number;
    ease?: Easing | Easing[];
    easings?: Easing[];
    // @internal
    elapsed?: number;
    flip?: number;
    from?: number | string;
    loop?: number;
    repeatDelay?: number;
    times?: number[];
    // @internal (undocumented)
    to?: number | string | ValueTarget;
    type?: "tween";
    // @internal (undocumented)
    velocity?: number;
    yoyo?: number;
}

// Warning: (ae-forgotten-export) The symbol "SyncLayoutProps" needs to be exported by the entry point index.d.ts
// Warning: (ae-internal-missing-underscore) The name "UnstableSyncLayout" should be prefixed with an underscore because the declaration is marked as @internal
// 
// @internal
export const UnstableSyncLayout: ({ children }: SyncLayoutProps) => JSX.Element;

// Warning: (ae-internal-missing-underscore) The name "unwrapMotionValue" should be prefixed with an underscore because the declaration is marked as @internal
// 
// @internal
export function unwrapMotionValue(value?: string | number | CustomValueType | MotionValue): string | number;

// @beta
export function useAnimatedState(initialState: any): any[];

// @public
export function useAnimation(): AnimationControls;

// Warning: (ae-forgotten-export) The symbol "CycleState" needs to be exported by the entry point index.d.ts
// 
// @public
export function useCycle<T>(...items: T[]): CycleState<T>;

// @public
export function useDomEvent(ref: RefObject<Element>, eventName: string, handler?: EventListener | undefined, options?: AddEventListenerOptions): void;

// @public
export function useDragControls(): DragControls;

// @public
export function useElementScroll(ref: RefObject<HTMLElement>): ScrollMotionValues;

// Warning: (ae-internal-missing-underscore) The name "useExternalRef" should be prefixed with an underscore because the declaration is marked as @internal
// 
// @internal
export function useExternalRef<E = Element>(externalRef?: Ref<E>): RefObject<E>;

// @public
export function useGestures<GestureHandlers>(props: GestureHandlers, ref: RefObject<Element>): void;

// Warning: (ae-forgotten-export) The symbol "ScaleMotionValues" needs to be exported by the entry point index.d.ts
// 
// @public
export function useInvertedScale(scale?: Partial<ScaleMotionValues>): ScaleMotionValues;

// @public
export function useMotionValue<T>(initial: T): MotionValue<T>;

// Warning: (ae-internal-missing-underscore) The name "usePanGesture" should be prefixed with an underscore because the declaration is marked as @internal
// 
// @internal (undocumented)
export function usePanGesture({ onPan, onPanStart, onPanEnd, onPanSessionStart }: PanHandlers, ref: RefObject<Element>): void;

// Warning: (ae-forgotten-export) The symbol "Present" needs to be exported by the entry point index.d.ts
// Warning: (ae-forgotten-export) The symbol "NotPresent" needs to be exported by the entry point index.d.ts
// 
// @public
export function usePresence(): Present | NotPresent;

// @public
export function useReducedMotion(): boolean;

// @public
export function useSpring(source: MotionValue | number, config?: SpringProps): MotionValue<any>;

// Warning: (ae-forgotten-export) The symbol "ControlsProp" needs to be exported by the entry point index.d.ts
// Warning: (ae-internal-missing-underscore) The name "useTapGesture" should be prefixed with an underscore because the declaration is marked as @internal
// 
// @internal (undocumented)
export function useTapGesture({ onTap, onTapStart, onTapCancel, whileTap, controls, }: TapHandlers & ControlsProp, ref: RefObject<Element>): void;

// Warning: (ae-forgotten-export) The symbol "Transformer" needs to be exported by the entry point index.d.ts
// 
// @public
export function useTransform<T>(parent: MotionValue, transform: Transformer_2<T>): MotionValue;

// @public
export function useTransform<T>(parent: MotionValue<number>, from: number[], to: T[], options?: TransformOptions<T>): MotionValue<T>;

// @public
export function useViewportScroll(): ScrollMotionValues;

// @public (undocumented)
export type ValueTarget = SingleTarget | KeyframesTarget;

// @public (undocumented)
export type Variant = TargetAndTransition | TargetResolver;

// @public
export type VariantLabels = string | string[];

// @public (undocumented)
export type Variants = {
    [key: string]: Variant;
};


// (No @packageDocumentation comment for this package)

```
