package com.cejv539.ebook.beans;

import java.io.Serializable;
import javax.enterprise.context.SessionScoped;
import javax.inject.Named;

/**
 *
 * @author Jianyu Feng
 */
@Named(value = "siteBean")
@SessionScoped
public class SiteBean implements Serializable {

    private String lastViewedBooks = "";
    private int lastViewedGenre;

    public String getLastViewedBooks() {
        return lastViewedBooks;
    }

    public void setLastViewedBooks(String lastViewedBooks) {
        this.lastViewedBooks = lastViewedBooks;
    }

    public int getLastViewedGenre() {
        return lastViewedGenre;
    }

    public void setLastViewedGenre(int lastViewedGenre) {
        this.lastViewedGenre = lastViewedGenre;
    }

}
