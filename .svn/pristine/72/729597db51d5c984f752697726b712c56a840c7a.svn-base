/*
 * 
 */
package com.cejv539.ebook;

import com.cejv539.ebook.beans.AdminPageBean;
import com.cejv539.ebook.beans.BookBean;
import com.cejv539.ebook.beans.CartBean;
import com.cejv539.ebook.beans.GenreBean;
import com.cejv539.ebook.beans.InventoryBean;
import com.cejv539.ebook.beans.InvoiceBean;
import com.cejv539.ebook.beans.ReportBean;
import com.cejv539.ebook.beans.SearchBean;
import com.cejv539.ebook.beans.SearchReviewBean;
import com.cejv539.ebook.beans.SiteBean;
import javax.inject.Inject;
import org.jboss.arquillian.container.test.api.Deployment;
import org.jboss.arquillian.junit.Arquillian;
import org.jboss.shrinkwrap.api.ArchivePaths;
import org.jboss.shrinkwrap.api.ShrinkWrap;
import org.jboss.shrinkwrap.api.asset.EmptyAsset;
import org.jboss.shrinkwrap.api.spec.WebArchive;
import static org.junit.Assert.assertNotNull;
import org.junit.Test;
import org.junit.runner.RunWith;

/**
 *
 * @author Jianyu Feng
 */
@RunWith(Arquillian.class)
public class DataBeanTest {

    @Inject
    BookBean bookBean;

    @Inject
    AdminPageBean adminPageBean;

    @Inject
    CartBean cartBean;

    @Inject
    GenreBean genreBean;

    @Inject
    InventoryBean inventoryBean;

    @Inject
    InvoiceBean invoiceBean;

    @Inject
    ReportBean reportBean;

    @Inject
    SearchBean searchBean;

    @Inject
    SearchReviewBean searchReviewBean;

    @Inject
    SiteBean siteBean;

    @Deployment
    public static WebArchive deploy() {
        return ShrinkWrap.create(WebArchive.class).
                addClasses(BookBean.class).
                addClasses(AdminPageBean.class).
                addClasses(CartBean.class).
                addClasses(GenreBean.class).
                addClasses(InventoryBean.class).
                addClasses(InvoiceBean.class).
                addClasses(ReportBean.class).
                addClasses(SearchBean.class).
                addClasses(SearchReviewBean.class).
                addClasses(SiteBean.class).
                addAsWebInfResource(EmptyAsset.INSTANCE,
                        ArchivePaths.create("beans.xml"));
    }

    @Test
    public void injection() {
        assertNotNull(bookBean);
        assertNotNull(adminPageBean);
        assertNotNull(cartBean);
        assertNotNull(genreBean);
        assertNotNull(inventoryBean);
        assertNotNull(invoiceBean);
        assertNotNull(reportBean);
        assertNotNull(searchBean);
        assertNotNull(searchReviewBean);
        assertNotNull(siteBean);

    }
}
