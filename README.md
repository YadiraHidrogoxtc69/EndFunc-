# EndFunc-
RegExpStringBetween(Const $test, Const $start_pattern, Const $end_pattern)     Local Const $start = StringRegExp($test, $start_pattern, 1)[0]      If @error Then Return SetError(1, 0, False)      Local Const $end = StringRegExp($test, $end_pattern, 1)[0]      If @error Then Return SetError(2, 0, False)      Local Const $string_between = _StringBetween($test, $start, $end)     Return @error ? SetError(3, 0, False) : $string_between EndFunc Edited January 2, 2014 by jaberwocky6669
