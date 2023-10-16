# roman-testing
import static org.junit.jupiter.api.Assertions.assertEquals;
import static org.junit.jupiter.api.Assertions.assertEquals;

import org.junit.jupiter.api.Test;

public class romantest {
    @Test
    public void shouldConvertromanToInteger() {
        assertEquals(1,new roman().romanToInt("I"));
        assertEquals(5, new roman().romanToInt("V"));
        assertEquals(10,new roman().romanToInt("X"));
        assertEquals(50,new roman().romanToInt("L"));
        assertEquals(100,new roman().romanToInt("C"));
        assertEquals(500,new roman().romanToInt("D"));
        assertEquals(1000, new roman().romanToInt("M"));
    }
    @Test
    public void shouldHandleSubtraction() {
        assertEquals(4,new roman().romanToInt("IV"));
        assertEquals(9,new roman().romanToInt("IX"));
        assertEquals(40,new roman().romanToInt("XL"));
        assertEquals(90,new roman().romanToInt("XC"));
        assertEquals(400,new roman().romanToInt("CD"));
        assertEquals(900,new roman().romanToInt("CM"));
    }
}
