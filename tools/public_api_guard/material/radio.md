## API Report File for "components-srcs"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { _AbstractConstructor } from '@angular/material/core';
import { AfterContentInit } from '@angular/core';
import { AfterViewInit } from '@angular/core';
import { BooleanInput } from '@angular/cdk/coercion';
import { CanDisableRipple } from '@angular/material/core';
import { ChangeDetectorRef } from '@angular/core';
import { _Constructor } from '@angular/material/core';
import { ControlValueAccessor } from '@angular/forms';
import { DoCheck } from '@angular/core';
import { ElementRef } from '@angular/core';
import { EventEmitter } from '@angular/core';
import { FocusMonitor } from '@angular/cdk/a11y';
import { FocusOrigin } from '@angular/cdk/a11y';
import { HasTabIndex } from '@angular/material/core';
import * as i0 from '@angular/core';
import * as i2 from '@angular/material/core';
import * as i3 from '@angular/common';
import { InjectionToken } from '@angular/core';
import { OnDestroy } from '@angular/core';
import { OnInit } from '@angular/core';
import { QueryList } from '@angular/core';
import { ThemePalette } from '@angular/material/core';
import { UniqueSelectionDispatcher } from '@angular/cdk/collections';

// @public (undocumented)
export const MAT_RADIO_DEFAULT_OPTIONS: InjectionToken<MatRadioDefaultOptions>;

// @public (undocumented)
export function MAT_RADIO_DEFAULT_OPTIONS_FACTORY(): MatRadioDefaultOptions;

// @public
export const MAT_RADIO_GROUP: InjectionToken<MatRadioGroup>;

// @public
export const MAT_RADIO_GROUP_CONTROL_VALUE_ACCESSOR: any;

// @public (undocumented)
export class MatRadioButton extends _MatRadioButtonMixinBase implements OnInit, AfterViewInit, DoCheck, OnDestroy, CanDisableRipple, HasTabIndex {
    constructor(radioGroup: MatRadioGroup, elementRef: ElementRef, _changeDetector: ChangeDetectorRef, _focusMonitor: FocusMonitor, _radioDispatcher: UniqueSelectionDispatcher, animationMode?: string, _providerOverride?: MatRadioDefaultOptions | undefined, tabIndex?: string);
    ariaDescribedby: string;
    ariaLabel: string;
    ariaLabelledby: string;
    readonly change: EventEmitter<MatRadioChange>;
    get checked(): boolean;
    set checked(value: BooleanInput);
    get color(): ThemePalette;
    set color(newValue: ThemePalette);
    get disabled(): boolean;
    set disabled(value: BooleanInput);
    focus(options?: FocusOptions, origin?: FocusOrigin): void;
    id: string;
    _inputElement: ElementRef<HTMLInputElement>;
    get inputId(): string;
    // (undocumented)
    _isRippleDisabled(): boolean;
    get labelPosition(): 'before' | 'after';
    set labelPosition(value: 'before' | 'after');
    _markForCheck(): void;
    name: string;
    // (undocumented)
    ngAfterViewInit(): void;
    // (undocumented)
    ngDoCheck(): void;
    // (undocumented)
    ngOnDestroy(): void;
    // (undocumented)
    ngOnInit(): void;
    _noopAnimations: boolean;
    // (undocumented)
    _onInputClick(event: Event): void;
    _onInputInteraction(event: Event): void;
    _onTouchTargetClick(event: Event): void;
    radioGroup: MatRadioGroup;
    get required(): boolean;
    set required(value: BooleanInput);
    protected _setDisabled(value: boolean): void;
    get value(): any;
    set value(value: any);
    // (undocumented)
    static ɵcmp: i0.ɵɵComponentDeclaration<MatRadioButton, "mat-radio-button", ["matRadioButton"], { "disableRipple": { "alias": "disableRipple"; "required": false; }; "tabIndex": { "alias": "tabIndex"; "required": false; }; "id": { "alias": "id"; "required": false; }; "name": { "alias": "name"; "required": false; }; "ariaLabel": { "alias": "aria-label"; "required": false; }; "ariaLabelledby": { "alias": "aria-labelledby"; "required": false; }; "ariaDescribedby": { "alias": "aria-describedby"; "required": false; }; "checked": { "alias": "checked"; "required": false; }; "value": { "alias": "value"; "required": false; }; "labelPosition": { "alias": "labelPosition"; "required": false; }; "disabled": { "alias": "disabled"; "required": false; }; "required": { "alias": "required"; "required": false; }; "color": { "alias": "color"; "required": false; }; }, { "change": "change"; }, never, ["*"], false, never>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatRadioButton, [{ optional: true; }, null, null, null, null, { optional: true; }, { optional: true; }, { attribute: "tabindex"; }]>;
}

// @public
export class MatRadioChange {
    constructor(
    source: MatRadioButton,
    value: any);
    source: MatRadioButton;
    value: any;
}

// @public (undocumented)
export interface MatRadioDefaultOptions {
    // (undocumented)
    color: ThemePalette;
}

// @public
export class MatRadioGroup implements AfterContentInit, OnDestroy, ControlValueAccessor {
    constructor(_changeDetector: ChangeDetectorRef);
    readonly change: EventEmitter<MatRadioChange>;
    // (undocumented)
    _checkSelectedRadioButton(): void;
    color: ThemePalette;
    _controlValueAccessorChangeFn: (value: any) => void;
    get disabled(): boolean;
    set disabled(value: BooleanInput);
    _emitChangeEvent(): void;
    get labelPosition(): 'before' | 'after';
    set labelPosition(v: 'before' | 'after');
    // (undocumented)
    _markRadiosForCheck(): void;
    get name(): string;
    set name(value: string);
    ngAfterContentInit(): void;
    // (undocumented)
    ngOnDestroy(): void;
    onTouched: () => any;
    _radios: QueryList<MatRadioButton>;
    registerOnChange(fn: (value: any) => void): void;
    registerOnTouched(fn: any): void;
    get required(): boolean;
    set required(value: BooleanInput);
    get selected(): MatRadioButton | null;
    set selected(selected: MatRadioButton | null);
    setDisabledState(isDisabled: boolean): void;
    _touch(): void;
    get value(): any;
    set value(newValue: any);
    writeValue(value: any): void;
    // (undocumented)
    static ɵdir: i0.ɵɵDirectiveDeclaration<MatRadioGroup, "mat-radio-group", ["matRadioGroup"], { "color": { "alias": "color"; "required": false; }; "name": { "alias": "name"; "required": false; }; "labelPosition": { "alias": "labelPosition"; "required": false; }; "value": { "alias": "value"; "required": false; }; "selected": { "alias": "selected"; "required": false; }; "disabled": { "alias": "disabled"; "required": false; }; "required": { "alias": "required"; "required": false; }; }, { "change": "change"; }, ["_radios"], never, false, never>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatRadioGroup, never>;
}

// @public (undocumented)
export class MatRadioModule {
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatRadioModule, never>;
    // (undocumented)
    static ɵinj: i0.ɵɵInjectorDeclaration<MatRadioModule>;
    // (undocumented)
    static ɵmod: i0.ɵɵNgModuleDeclaration<MatRadioModule, [typeof i1.MatRadioGroup, typeof i1.MatRadioButton], [typeof i2.MatCommonModule, typeof i3.CommonModule, typeof i2.MatRippleModule], [typeof i2.MatCommonModule, typeof i1.MatRadioGroup, typeof i1.MatRadioButton]>;
}

// (No @packageDocumentation comment for this package)

```
